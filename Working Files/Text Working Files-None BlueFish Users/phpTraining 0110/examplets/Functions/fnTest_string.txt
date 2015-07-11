<style type="text/css">
body {
	font-family: Arial, Helvetica, sans-serif;
}
.scriptcolour {
	color: maroon;	
}
</style>

<?php
//fnTest_strings.php

echo '<p>Examples of php built-in string functions</p>';

echo "<br /><hr /><br />";

$p = fnTestString('chr(67)', 'Return a specific character');

$p = fnTestString('"*".ltrim(" \t trimmed")', 'Strip whitespace from the beginning of a string');
$p = fnTestString('md5("fred")', 'Calculate the md5 hash of a string');

$p = fnTestString('number_format("7782975.8988",2, ".",",")', 'Format a number with grouped thousands');
$p = fnTestString('ord("f")', 'Return ASCII value of character');

$p = fnTestString('rtrim("trimmed \t ")."*"', 'Strip whitespace (or other characters) from the end of a string');
$p = fnTestString('str_ireplace("x","y","PxPXPxpppx")', 'Case-insensitive version of str_replace.');
$p = fnTestString('str_pad("xyz",10, "0")', 'Pad a string to a certain length with another string');
$p = fnTestString('str_repeat("-",12)', 'Repeat a string');
$p = fnTestString('str_replace("x","y","PxPXPxpppx")', 'Replace all occurrences of the search string with the replacement string');
echo "<br /><hr /><br />";
$p = fnTestString('strip_tags("*<p>test para</p><br />*")', 'Strip HTML and PHP tags from a string');
echo "<br /><hr /><br />";
$p = fnTestString('strlen("This is how long?")', 'Get string length');
$p = fnTestString('strpos("abcdefg","d")', 'Find position of first occurrence of a string');
$p = fnTestString('strrev("abcd")', 'Reverse a string');
$p = fnTestString('strtolower("AbCdEfG")', 'Make a string lowercase');
$p = fnTestString('strtoupper("AbCdEfG")', 'Make a string uppercase');
echo "<br /><hr /><br />";
$p = fnTestString('substr("abcdefghij",2,3)', 'Return part of a string');
$p = fnTestString('substr("abcdefghij",-4)', 'Return part of a string');
$p = fnTestString('substr("abcdefghij", 3)', 'Return part of a string');
echo "<br /><hr /><br />";
$p = fnTestString('"*".trim(" \t xyz \t ")."*"', 'Strip whitespace (or other characters) from the beginning and end of a string');
$p = fnTestString('ucfirst("mr fred smith")', 'Make a strings first character uppercase');
$p = fnTestString('ucwords("mr fred smith")', 'Uppercase the first character of each word in a string');

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