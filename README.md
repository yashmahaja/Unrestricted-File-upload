# Unrestricted-File-upload

-> Bypass Client Side Validation
Intercept request in burp -> modify request change extension to php,svg -> send request to server

-> Double Extension Attack: uploading file as shell.php.jpg/shell.jpg.php

-> NullByte Injection: shell.php%00.jpg

-> put file name ../../logo.png or ../../etc/passwd/logo.png to get directory traversal via upload file

-> Upload large size file for DoS attack test using the image.

-> (magic number) upload shell.php change content-type to image/gif and start content with GIF89a; will do the job!

-> upload the file using SQL command ‘sleep(10).jpg you may achieve SQL if image directly saves to DB.

-> If web app allows for zip upload then rename the file to pwd.jpg bcoz developer handle it via command
