You can now test the installation by entering either of the following URLs into your
web browser to call up the screen shown in Figure 2-18:
 http://localhost:10088
 http://127.0.0.1:10088

The word localhost specifies the local computer, which will also respond to the IP
address 127.0.0.1. The reason for entering :10088 is because many Mac computers will
already have a web server running: adding this avoids any clashes. You must therefore
remember to place :10088 after every http://localhost for all examples in this book. So,
for example, if the filename test.php is being used, you would call it up from the browser
using the URL http://localhost:10088/test.php.

If you are sure that there isn’t another web server running on your Mac
you can edit the configuration file at the following location (ensuring
you have permission to do so), changing the command (at about line
40) that reads Listen 10088 to Listen 80:
/usr/local/zend/apache2/conf/httpd.conf
You will then need to restart the server by opening the Terminal utility
and issuing the following command:
sudo /usr/local/zend/bin/zendctl.sh restart
Now you will no longer need to add the :10088 to local URLs.
The page that gets displayed in the browser when you go to http://localhost or http://
localhost:10088 is the file index.html in the server’s document root, which is the direc-
tory that contains the main web documents for a domain. This is the one that is entered

[Previous](\Configuring MySQL.md) [Next]
