<?php

$uploadActivated = $_POST['uploadActivated'];

if (isset($uploadActivated) AND $uploadActivated == 1) {
	
	$uploaddir = '../images/';
	$uploadfile = $uploaddir . basename($_FILES['userfile']['name']);
	

	if (move_uploaded_file($_FILES['userfile']['tmp_name'], $uploadfile)) {
		 chmod($uploadfile, 0666);			//		used for commercial grade systems 		
	    echo "File is valid, and was successfully uploaded.<br />";

		echo 'The image uploaded was "'.$uploadfile.'"<br /><br /><br />';	
		echo '<img src="'.$uploadfile.'" alt="Test Image uploaded" />';

	} else {
	    echo "File upload error!<br />";
	}
		
	unset($uploadActivated);	
		
}

		
echo '
<!-- The data encoding type, enctype, MUST be specified as below -->
<form enctype="multipart/form-data" action="uploadtest.php" method="POST">
    <!-- MAX_FILE_SIZE must precede the file input field -->
    <input type="hidden" name="uploadActivated" value=1 />
    
    <input type="hidden" name="MAX_FILE_SIZE" value="300000" />
    <!-- Name of input element determines name in $_FILES array -->
    Send this file: <input name="userfile" type="file" />
    <input type="submit" value="Upload File" />
</form>';
	
	

?>