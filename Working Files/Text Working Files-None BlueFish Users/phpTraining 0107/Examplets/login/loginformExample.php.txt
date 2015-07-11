<?php
	
//		File in DEMO folder:              loginformExample.php
echo '<h2>Login Form Example:</h2>';

	$username = $_POST['username'];
	if(isset($username)) {
		$password = $_POST['password'];
		echo "username = ".$username."<br />";
		echo "password = ".$password."<br />";

		unset($username);
		unset($password);
	} 

	echo '<form name="postLogin" action="loginformExample.php" method="post">';	
			echo '
				<P>User name: 
				<INPUT TYPE=text NAME=username value="" SIZE=12 MAXLENGTH=8></P>
				<P>Password: 
				<INPUT TYPE=text NAME=password value="" SIZE=12 MAXLENGTH=12></P>
				<input type="submit"  value="Login" />
			';
	echo '</form>';
	echo '<br /><hr /><br />';

	echo '<form name="postLoginHid" action="loginformExample.php" method="post">';	
			echo '
				<P>User name: 
				<INPUT TYPE=text NAME=username value="" SIZE=12 MAXLENGTH=16></P>
				<P>Password: 
				<INPUT TYPE=password NAME=password value="" SIZE=12 MAXLENGTH=16></P>
				<input type="submit"  value="Login" />
			';
	echo '</form>';

echo '<h2>--------- END Login Form --------</h2>';

?>