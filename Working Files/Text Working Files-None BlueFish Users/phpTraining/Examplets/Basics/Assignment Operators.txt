<?php
	
/*

*	File:		phpOperatorsAssig.php
*	By:		TMIT
*	Date:		2010-07-05
*
*	This script demonstrates php Assignment Operators
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

	echo "<span style=\"color:red;\"><strong>Assignment Operators</strong><br /></span><br /><br />";

	echo " = , += , -= , *= , /= , %=  , .= <br /><br />";
	
	$x = 3; $y = 4;
	echo "<u>CODE: - demonstrating assignment operator '+='</u><br />";
	echo "	\$x = ".$x.";  \$y = ".$y.";<br />";
	echo "\$y += \$x;  &nbsp;&nbsp;&nbsp; // (same as \$y = \$y + \$x )<br />";
	echo "\$result = \$y; <br />";
	echo "echo \"result = \".\$result; <br />";
	echo "-------------------------------------------<br />";	
	$y += $x;
	$result = $y;
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";

	$x = 3; $y = 4;
	echo "<u>CODE: - demonstrating assignment operator '-='</u><br />";
	echo "	\$x = ".$x.";  \$y = ".$y.";<br />";
	echo "\$y -= \$x;  &nbsp;&nbsp;&nbsp; // (same as \$y = \$y - \$x )<br />";
	echo "\$result = \$y; <br />";
	echo "echo \"result = \".\$result; <br />";
	echo "-------------------------------------------<br />";	
	$y -= $x;
	$result = $y;
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";

	$x = 3; $y = 4;
	echo "<u>CODE: - demonstrating assignment operator '*='</u><br />";
	echo "	\$x = ".$x.";  \$y = ".$y.";<br />";
	echo "\$y *= \$x;  &nbsp;&nbsp;&nbsp; // (same as \$y = \$y * \$x )<br />";
	echo "\$result = \$y; <br />";
	echo "echo \"result = \".\$result; <br />";
	echo "-------------------------------------------<br />";	
	$y *= $x;
	$result = $y;
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";

	$x = 3; $y = 414;
	echo "<u>CODE: - demonstrating assignment operator '/='</u><br />";
	echo "	\$x = ".$x.";  \$y = ".$y.";<br />";
	echo "\$y /= \$x;  &nbsp;&nbsp;&nbsp; // (same as \$y = \$y / \$x )<br />";
	echo "\$result = \$y; <br />";
	echo "echo \"result = \".\$result; <br />";
	echo "-------------------------------------------<br />";	
	$y /= $x;
	$result = $y;
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";

	$x = 17; $y = 39;
	echo "<u>CODE: - demonstrating assignment operator '%='</u><br />";
	echo "	\$x = ".$x.";  \$y = ".$y.";<br />";
	echo "\$y %= \$x; &nbsp;&nbsp;&nbsp; // (remainder of ".$y." / ".$x."<br />";
	echo "\$result = \$y; <br />";
	echo "echo \"result = \".\$result; <br />";
	echo "-------------------------------------------<br />";	
	$y %= $x;
	$result = $y;
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";

	echo "<span style=\"color:red;\"><strong>Concatenation</strong><br /></span><br /><br />";

	$x = "First part "; $y = "Second part ";
	echo "<u>CODE: - demonstrating assignment operator '.=' for strings</u><br />";
	echo "	\$x = ".$x.";  \$y = ".$y.";<br />";
	echo "\$y .= \$x; <br />";
	echo "\$result = \$y; <br />";
	echo "echo \"result = \".\$result; <br />";
	echo "-------------------------------------------<br />";	
	$y .= $x;
	$result = $y;
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";


	$x = 7.3; $y = 8.6;
	echo "<u>CODE: - demonstrating assignment operator '.=' for numbers</u><br />";
	echo "	\$x = ".$x.";  \$y = ".$y.";<br />";
	echo "\$y .= \$x; <br />";
	echo "\$result = \$y; <br />";
	echo "echo \"result = \".\$result; <br />";
	echo "-------------------------------------------<br />";	
	$y .= $x;
	$result = $y;
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";



}

echo "</div>";

?>