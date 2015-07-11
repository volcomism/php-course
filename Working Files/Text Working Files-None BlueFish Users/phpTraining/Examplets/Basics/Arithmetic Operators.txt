<?php
	
/*

*	File:		phpOperatorsArith.php
*	By:		TMIT
*	Date:		2010-07-05
*
*	This script demonstrates php Arithmetic Operators
*
*
*
*=====================================
*/

{
	echo "<p >There's a whole load of examples here to demonstrate ";
	echo "variables and operators in php.</p>";
	echo "<br /><hr /><br />";
	
	echo "Notice in the code how some special characters ($ of variables and double quotes) ";
	echo "in the echo statements need to be 'escaped' ";
	echo "with the backslash ";
	echo "so that they are not interpreted as part of the php code.<br /><br />";
}
echo "<div style=\"padding-left: 60px; font-family: Arial, Helvetica, sans-serif;\">";
{ //     Arithmetic Operators

	echo "<span style=\"color:red;\"><strong>Arithmetic Operators</strong><br /></span><br />";

	$x = 3; $y = 4;
	$result = $x + $y;
	echo "<u>CODE: - demonstrating binary operator '+'</u><br />";
	echo "	\$x = ".$x.";  \$y = ".$y.";<br />";
	echo "\$result = \$x + \$y; <br />";
	echo "echo \"result = \".\$result; <br />";
	echo "-------------------------------------------<br />";	
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";


	$x = 13; $y = 4;
	$result = $x - $y;
	echo "<u>CODE: - demonstrating binary operator '-'</u><br />";
	echo "	\$x = ".$x.";  \$y = ".$y.";<br />";
	echo "	\$result = \$x - \$y;<br />";
	echo "	echo \"result = \".\$result;<br />";
	echo "-------------------------------------------<br />";
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";


	$x = 3; $y = 4;
	$result = $x * $y;
	echo "<u>CODE: - demonstrating binary operator '*'</u><br />";
	echo "	\$x = ".$x.";  \$y = ".$y.";<br />";
	echo "	\$result = \$x * \$y;<br />";
	echo "	echo \"result = \".\$result;<br />";
	echo "-------------------------------------------<br />";
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";


	$x = 18;  $y = 3;
	$result = $x / $y;
	echo "<u>CODE: - demonstrating binary operator '/'</u><br />";
	echo "	\$x = ".$x.";  \$y = ".$y.";<br />";
	echo "	\$result = \$x / \$y;<br />";
	echo "	echo \"result = \".\$result;<br />";
	echo "-------------------------------------------<br />";
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";


	$x = 13;  $y = 5;
	$result = $x % $y;
	echo "<u>CODE: - demonstrating binary operator '%'</u><br />";
	echo "	\$x = ".$x.";  \$y = ".$y.";<br />";
	echo "	\$result = \$x % \$y;<br />";
	echo "	echo \"result = \".\$result;<br />";
	echo "-------------------------------------------<br />";
	echo "result = ".$result." &nbsp;&nbsp;&nbsp;(ie. remainder when ".$x." divided by ".$y." )";
	echo "<br />===========================================<br /><br />";


	$x = 13;
	echo "<u>CODE: - demonstrating UNARY operator '++'</u><br />";
	echo "	\$x = ".$x.";<br />";
	$x++;
	$result = $x;
	echo "	\$x++;<br />";
	echo "	\$result = \$x;<br />";
	echo "	echo \"result = \".\$result;<br />";
	echo "-------------------------------------------<br />";
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";

	$x = 13;
	echo "<u>CODE: - demonstrating UNARY operator '--'</u><br />";
	echo "	\$x = ".$x.";<br />";
	$x--;
	$result = $x;
	echo "	\$x--;<br />";
	echo "	\$result = \$x;<br />";
	echo "	echo \"result = \".\$result;<br />";
	echo "-------------------------------------------<br />";
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";



}

echo "</div>";

?>