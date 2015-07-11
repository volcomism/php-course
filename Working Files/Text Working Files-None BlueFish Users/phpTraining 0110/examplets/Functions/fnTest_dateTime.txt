<style type="text/css">
body {
	font-family: Arial, Helvetica, sans-serif;
}
.scriptcolour {
	color: maroon;	
}
</style>
<?php

echo '<p>Examples of php built-in date functions</p>';

echo "<br /><hr /><br />";

$p = fnTestString('strtotime("now")', 'format NOW to UNIX format');
$p = fnTestString('time()', 'format NOW to UNIX microtime format');
$p = fnTestString('microtime()', 'format NOW to UNIX microtime format');

echo "<br /><hr /><br />";

$p = fnTestString('date("Y-m-d H:i:s", strtotime("now"))', 'format NOW to MySQL format');
$p = fnTestString('date("Y-m-d H:i:s")', 'format NOW to MySQL format');
echo "<br /><hr /><br />";

$p = fnTestString('date("D j M Y H:i:s", strtotime("+2 hours"))', 'format 2 hours hence to human format');
$p = fnTestString('date("D j M Y H:i:s", strtotime("+7 days"))', 'format 7 days hence to human format');

echo "<br /><hr /><br />";

$p = fnTestString('date("D j M Y H:i:s", strtotime("tomorrow"))', 'format tomorrow to human format');
$p = fnTestString('date("D j M Y H:i:s", strtotime("+1 day"))', 'format tomorrow to human format');
echo "<br /><hr /><br />";

$p = fnTestString('date("D j M Y H:i:s", strtotime("yesterday"))', 'format yesterday to human format');
$p = fnTestString('date("D j M Y H:i:s", strtotime("-1 day"))', 'format yesterday to human format');

echo "<br /><hr /><br />";

$p = fnTestString('date("g:i A, D j M Y", strtotime("yesterday"))', 'format yesterday to 12 hour format');
$p = fnTestString('date("g:i A, D j M Y", strtotime("-1 day"))', 'format yesterday to 12 hour format');



function fnTestString($fn, $meaning) {
	
	echo eval('$p = '.$fn.';');
	echo '<p>'.$meaning.':  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
		<span class="scriptcolour">
		echo '.$fn.'; </span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
		<span style="color: blue">';
	echo $p;
	echo '</p></span>';
}

?>