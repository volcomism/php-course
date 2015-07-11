<?php
	
/*

*	File:		phpOperatorsCompare.php
*	By:		TMIT
*	Date:		2010-07-05
*
*	This script demonstrates php Comparison Operators
*
*
*
*=====================================
*/

{
	echo "<p >There's a whole load of examples here to demonstrate ";
	echo "variables and operators in php.</p>";
	echo "<br /><hr /><br />";
	
	echo "Notice 'escaped' characters<br />";
	echo "\\\" to escape double quotes<br />";
	echo "\\\$ to escape a dollar symbol<br />";
	echo "and the use of '&amp;nbsp;' to force a non-breaking space.<br />";
	
	echo "so that they are not interpreted as part of the php code.<br /><br />";
}
echo "<div style=\"padding-left: 60px; font-family: Arial, Helvetica, sans-serif;\">";
{ //     Comparison Operators

	echo "<span style=\"color:red;\"><strong>Comparison Operators</strong><br /></span><br /><br />";

	echo " == , < , <= , > , >= , != , <> <br /><br />";
	
	$x = 3; $y = 4;	
	if ($x == $y) {
		$result = "TRUE";
	} else {
		$result = "FALSE";
	}	
	echo "<u>CODE: - demonstrating Comparison operator ' == '</u><br />";	
	echo "	\$x = ".$x.";  \$y = ".$y.";<br />";
	echo "	if (\$x == \$y) {&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;";
	echo "	// &nbsp;&nbsp;&nbsp; << REMEMBER THIS ! &nbsp;&nbsp;&nbsp;  it's ";
	echo "	<span style=\"color:red;\"><strong>==</strong></span><br />";
	echo "	&nbsp;&nbsp;&nbsp;&nbsp;\$result = \"TRUE\";<br />";
	echo "	} else {<br />";
	echo "	&nbsp;&nbsp;&nbsp;&nbsp;\$result = \"FALSE\";<br />";
	echo "	}<br />";
	echo "	echo \"result = \".\$result;<br />";
	echo "-------------------------------------------<br />";	
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";

	$x = 3; $y = 4;	
	if ($x < $y) {
		$result = "TRUE";
	} else {
		$result = "FALSE";
	}	
	echo "<u>CODE: - demonstrating Comparison operator ' < '</u><br />";	
	echo "	\$x = ".$x.";  \$y = ".$y.";<br />";
	echo "	if (\$x < \$y) {<br />";
	echo "	&nbsp;&nbsp;&nbsp;&nbsp;\$result = \"TRUE\";<br />";
	echo "	} else {<br />";
	echo "	&nbsp;&nbsp;&nbsp;&nbsp;\$result = \"FALSE\";<br />";
	echo "	}<br />";
	echo "	echo \"result = \".\$result;<br />";
	echo "-------------------------------------------<br />";	
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";

	$x = 3; $y = 4;	
	if ($x <= $y) {
		$result = "TRUE";
	} else {
		$result = "FALSE";
	}	
	echo "<u>CODE: - demonstrating Comparison operator ' <= '</u><br />";	
	echo "	\$x = ".$x.";  \$y = ".$y.";<br />";
	echo "	if (\$x <= \$y) {<br />";
	echo "	&nbsp;&nbsp;&nbsp;&nbsp;\$result = \"TRUE\";<br />";
	echo "	} else {<br />";
	echo "	&nbsp;&nbsp;&nbsp;&nbsp;\$result = \"FALSE\";<br />";
	echo "	}<br />";
	echo "	echo \"result = \".\$result;<br />";
	echo "-------------------------------------------<br />";	
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";

	$x = 3; $y = 4;	
	if ($x > $y) {
		$result = "TRUE";
	} else {
		$result = "FALSE";
	}	
	echo "<u>CODE: - demonstrating Comparison operator ' > '</u><br />";	
	echo "	\$x = ".$x.";  \$y = ".$y.";<br />";
	echo "	if (\$x > \$y) {<br />";
	echo "	&nbsp;&nbsp;&nbsp;&nbsp;\$result = \"TRUE\";<br />";
	echo "	} else {<br />";
	echo "	&nbsp;&nbsp;&nbsp;&nbsp;\$result = \"FALSE\";<br />";
	echo "	}<br />";
	echo "	echo \"result = \".\$result;<br />";
	echo "-------------------------------------------<br />";	
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";

	$x = 3; $y = 4;	
	if ($x >= $y) {
		$result = "TRUE";
	} else {
		$result = "FALSE";
	}	
	echo "<u>CODE: - demonstrating Comparison operator ' >= '</u><br />";	
	echo "	\$x = ".$x.";  \$y = ".$y.";<br />";
	echo "	if (\$x >= \$y) {<br />";
	echo "	&nbsp;&nbsp;&nbsp;&nbsp;\$result = \"TRUE\";<br />";
	echo "	} else {<br />";
	echo "	&nbsp;&nbsp;&nbsp;&nbsp;\$result = \"FALSE\";<br />";
	echo "	}<br />";
	echo "	echo \"result = \".\$result;<br />";
	echo "-------------------------------------------<br />";	
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";

	
	$x = 3; $y = 4;	
	if ($x != $y) {
		$result = "TRUE";
	} else {
		$result = "FALSE";
	}	
	echo "<u>CODE: - demonstrating Comparison operator ' != '</u><br />";	
	echo "	\$x = ".$x.";  \$y = ".$y.";<br />";
	echo "	if (\$x != \$y) {<br />";
	echo "	&nbsp;&nbsp;&nbsp;&nbsp;\$result = \"TRUE\";<br />";
	echo "	} else {<br />";
	echo "	&nbsp;&nbsp;&nbsp;&nbsp;\$result = \"FALSE\";<br />";
	echo "	}<br />";
	echo "	echo \"result = \".\$result;<br />";
	echo "-------------------------------------------<br />";	
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";

	$x = 3; $y = 4;	
	if ($x <> $y) {
		$result = "TRUE";
	} else {
		$result = "FALSE";
	}	
	echo "<u>CODE: - demonstrating Comparison operator ' <> '</u><br />";	
	echo "	\$x = ".$x.";  \$y = ".$y.";<br />";
	echo "	if (\$x <> \$y) {<br />";
	echo "	&nbsp;&nbsp;&nbsp;&nbsp;\$result = \"TRUE\";<br />";
	echo "	} else {<br />";
	echo "	&nbsp;&nbsp;&nbsp;&nbsp;\$result = \"FALSE\";<br />";
	echo "	}<br />";
	echo "	echo \"result = \".\$result;<br />";
	echo "-------------------------------------------<br />";	
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";



}

echo "</div>";

?>