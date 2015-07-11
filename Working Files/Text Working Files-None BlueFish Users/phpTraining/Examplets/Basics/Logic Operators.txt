<?php
/*

*	File:		phpOperatorsLogic.php
*	By:		TMIT
*	Date:		2010-07-05
*
*	This script demonstrates php Logic Operators
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

{ //     Logic Operators

	echo "<span style=\"color:red;\"><strong>LOGIC Operators</strong><br /></span><br />";

	$x = TRUE; $y = FALSE;
	$result = $x && $y;
	echo "<u>CODE: - demonstrating LOGIC operator '&&'</u><br />";
	echo "	\$x = TRUE;  \$y = FALSE;<br />";
	echo "\$result = \$x && \$y; <br />";
	echo "echo \"result = \".\$result; <br />";
	echo "-------------------------------------------<br />";	
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";

	$x = TRUE; $y = TRUE;
	$result = $x AND $y;
	echo "<u>CODE: - demonstrating LOGIC operator 'AND'</u><br />";
	echo "	\$x = TRUE;  \$y = TRUE;<br />";
	echo "\$result = \$x AND \$y; <br />";
	echo "echo \"result = \".\$result; <br />";
	echo "-------------------------------------------<br />";	
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";

	$x = FALSE; $y = FALSE;
	$result = $x && $y;
	echo "<u>CODE: - demonstrating LOGIC operator '&&'</u><br />";
	echo "	\$x = FALSE;  \$y = FALSE;<br />";
	echo "\$result = \$x && \$y; <br />";
	echo "echo \"result = \".\$result; <br />";
	echo "-------------------------------------------<br />";	
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";


	$x = NULL; $y = FALSE;
	$result = $x && $y;
	echo "<u>CODE: - demonstrating LOGIC operator '&&'</u><br />";
	echo "	\$x = NULL;  \$y = FALSE;<br />";
	echo "\$result = \$x && \$y; <br />";
	echo "echo \"result = \".\$result; <br />";
	echo "-------------------------------------------<br />";	
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";

	//						OR operator

	$x = TRUE; $y = FALSE;
	$result = $x || $y;
	echo "<u>CODE: - demonstrating LOGIC operator '||'</u><br />";
	echo "	\$x = TRUE;  \$y = FALSE;<br />";
	echo "\$result = \$x || \$y; <br />";
	echo "echo \"result = \".\$result; <br />";
	echo "-------------------------------------------<br />";	
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";

	$x = TRUE; $y = TRUE;
	$result = $x OR $y;
	echo "<u>CODE: - demonstrating LOGIC operator 'OR'</u><br />";
	echo "	\$x = TRUE;  \$y = TRUE;<br />";
	echo "\$result = \$x OR \$y; <br />";
	echo "echo \"result = \".\$result; <br />";
	echo "-------------------------------------------<br />";	
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";

	$x = FALSE; $y = FALSE;
	$result = $x || $y;
	echo "<u>CODE: - demonstrating LOGIC operator '||'</u><br />";
	echo "	\$x = FALSE;  \$y = FALSE;<br />";
	echo "\$result = \$x || \$y; <br />";
	echo "echo \"result = \".\$result; <br />";
	echo "-------------------------------------------<br />";	
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";


	$x = NULL; $y = FALSE;
	$result = $x || $y;
	echo "<u>CODE: - demonstrating LOGIC operator '||'</u><br />";
	echo "	\$x = NULL;  \$y = FALSE;<br />";
	echo "\$result = \$x || \$y; <br />";
	echo "echo \"result = \".\$result; <br />";
	echo "-------------------------------------------<br />";	
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";

	//						NOT operator   or    !

	$x = TRUE;
	$result = !$x;
	echo "<u>CODE: - demonstrating LOGIC operator '!' ie the NOT operator</u><br />";
	echo "	\$x = TRUE;<br />";
	echo "\$result = !\$x; <br />";
	echo "echo \"result = \".\$result; <br />";
	echo "-------------------------------------------<br />";	
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";

	$x = FALSE;
	$result = !$x;
	echo "<u>CODE: - demonstrating LOGIC operator '!' ie the NOT operator</u><br />";
	echo "	\$x = TRUE;<br />";
	echo "\$result = !\$x; <br />";
	echo "echo \"result = \".\$result; <br />";
	echo "-------------------------------------------<br />";	
	echo "result = ".$result;
	echo "<br />===========================================<br /><br />";

}


echo "</div>";

?>