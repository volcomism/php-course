<style type="text/css">
body {
	font-family: Arial, Helvetica, sans-serif;
}
.scriptcolour {
	color: maroon;	
}
</style>

<?php

echo '<p>Examples of php built-in maths functions</p>';

echo "<br /><hr /><br />";

$p = fnTestString("Absolute value", "abs(-7.5)");
$p = fnTestString("Round fractions up", "ceil(2.49999999)");
$p = fnTestString("Round fractions down", "floor(2.4999999999999999999999)");
$p = fnTestString("Find highest value", "max(2.5, 14, 17, 1, 19)");
$p = fnTestString("Find lowest value", "min(2.5, 14, 17, 1, 19)");
$p = fnTestString("Generate random value", "mt_rand()");
$p = fnTestString("Rounds a float", "round(2.59)");
$p = fnTestString("Square root", "sqrt(81.8)");



function fnTestString($meaning, $fn) {
	
	echo eval('$p = '.$fn.';');
	echo '<p>'.$meaning.':  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
		<span class="scriptcolour">
		echo '.$fn.'; </span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
		<span style="color: blue">';
	echo $p;
	echo '</p></span>';
}

?>   