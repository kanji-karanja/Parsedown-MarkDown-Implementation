# Parsedown-MarkDown-Implementation in PHP

**Done in PHP**

This is a simple project that can read a MARKDOWN file then output it as HTML.

Can have several applications.

Uses ParseDown Library to do the server side parsing.

```PHP
<?php
require 'Parsedown.php';
$Parsedown = new Parsedown();
$myfile = fopen("EXAMPLE.md", "r") or die("Unable to open file!");
echo $Parsedown->text(fread($myfile,filesize("EXAMPLE.md")));
fclose($myfile);
?>
```
