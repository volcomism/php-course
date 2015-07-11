<?php

echo "fnTest_args_01<br /><br />";

function twoArgs($x, $y) {
	echo "twoArgs<br />";
	echo '<p>x : '.$x.'</p>';
	echo '<p>y : '.$y.'</p>';	
	echo '<p>z : '.$z.'</p>';
	echo "------------------<br />";
}

function optionalArgs($x, $y = 12, $z = 24) {
	echo "optionalArgs<br />";
	echo '<p>x : '.$x.'</p>';
	echo '<p>y : '.$y.'</p>';	
	echo '<p>z : '.$z.'</p>';
	echo "------------------<br />";
}


	$p = optionalArgs(2);
	$q = optionalArgs(2, 3);
	$r = optionalArgs(2, 3, 4);
	$r = optionalArgs(2, 3, 4, 5);

echo "<br /><hr /><br />";
	
	$p = twoArgs(2);
	$q = twoArgs(2, 3);
	$r = twoArgs(2, 3, 4);
	$r = twoArgs(2, 3, 4, 5);

?>