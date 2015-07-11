<?php

//		getFileContents.php


$urlString = 'http://www.training.tmit.net/tmit/tempHTML/toowhoo.html';

$pageContent = file_get_contents($urlString);

				$pageContent = str_replace("<","&lt;",$pageContent);
				$pageContent = str_replace(">","&gt;<br />",$pageContent);

echo $pageContent;



?>