<?php
	
/*

*	INCLUDE File:          stringFunctions.php
*	By:							TMIT
*	Date:		
*
*	String Functions for project "ALPHA CRM" 
*
*
*=====================================
*/


		function fullCoName($coID, $preName, $coName, $regType)
		{
			if (empty($coID)) {
				$temp = "Un-Allocated";
			} else {
				$temp = trim($preName." ".$coName." ".$regType);
			}
			return $temp;
		}


		function shortCoName($coName, $regType)
		{
			$temp = trim($coName." ".$regType);
			return $temp;
		}

		function coAddress($A, $B, $C)
		{
			$temp = $A;
			if (!empty($B)) { $temp .=  ", ".$B; }
			if (!empty($C)) { $temp .=  ", ".$C; }
			return $temp;
		}


?>