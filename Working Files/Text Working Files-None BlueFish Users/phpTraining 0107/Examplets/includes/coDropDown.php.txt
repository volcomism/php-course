<?php
	
/*

*	INCLUDE File:          coDropDown.php
*	By:							TMIT
*	Date:		
*
*	code to render a dropDown for companies
*		and send the companyID to the script $postFormName
*		as a POSTed variable.
*
*
*=====================================
*/
				
		$tCompany_SQLselect = "SELECT  ";
		$tCompany_SQLselect .= "ID, preName, Name ";	
		$tCompany_SQLselect .= "FROM ";
		$tCompany_SQLselect .= "tCompany ";
		$tCompany_SQLselect .= "Order By Name ";
			
		$tCompany_SQLselect_Query = mysql_query($tCompany_SQLselect);	
		
		echo '<form action="'.$postFormName.'" method="post">';
		
		echo '<select name="companyID">';
		
			echo '<option value="0" label="coyvalue" selected="selected">..select company..</option>';
	 	
				while ($row = mysql_fetch_array($tCompany_SQLselect_Query, MYSQL_ASSOC)) {
				    $ID = $row['ID'];
				    $preName = $row['preName'];
				    $companyName = $row['Name'];
				    $RegType = $row['RegType'];
				    
				    $fullCoyName = trim($preName." ".$companyName." ".$RegType);
				    
				    echo '<option value="'.$ID.'">'.$fullCoyName.'</option>';
				}
			
				mysql_free_result($tCompany_SQLselect_Query);		
		
				echo '</select>';
		
				echo '<input type="submit" />';
				
		echo '</form>';
		//	END:  Select company from dropdowm

?>