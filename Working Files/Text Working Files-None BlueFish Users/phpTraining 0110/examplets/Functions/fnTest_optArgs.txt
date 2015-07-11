<?php

echo "fnTest_optionalArgs_01<br /><br />";

function noArgs() {
	echo "function noArgs() &nbsp;&nbsp;&nbsp;";
  if (func_num_args() == 0) {
    return false;
    }
  else {
    for ($i =0; $i < func_num_args(); $i++) {
      $x = func_get_arg($i);
 			echo $x;
      }
    }
  echo "<br /><hr /><br />";

  }


	$p = noArgs(2);
	$q = noArgs(2, 3);
	$r = noArgs(2, "x", 4);
	$r = noArgs(2, "p", 4, "q");

echo "<br /><hr /><br />";


?>