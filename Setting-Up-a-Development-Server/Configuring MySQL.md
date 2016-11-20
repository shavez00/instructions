Now that we've learned about the windows terminal and the windows directory structure it's time to finish setting up our development server.  Even though our MySQL server has been installed will need to go into the terminal and configure it.

Unfortunately, the Zend Server CE installer doesn’t set up the commands needed to be
able to start, stop, and restart the MySQL server, so you’re going to have to do this
manually by opening a Terminal window and entering the following command:
 sudo nano /usr/local/zend/bin/zendctl.sh

After entering your password you will now be in the Nano text editor, so move the
cursor down a few lines using the down arrow key and, where you see the line that
reads MySQL_EN="false", change the word false to true.
Now scroll down some more until you find these two lines:
case $1 in
        "start")
Below them you’ll see an indented line that reads:
                $0 start-apache
Just after this line, insert a new one that reads as follows:
                $0 start-MySQL
This will allow MySQL to start. Now scroll down a little more until you get to the
section that starts:
        "restart")
Below it you’ll see an indented line that reads:
                $0 restart-apache

Just after this line, insert a new one that reads as follows:
                $0 restart-MySQL

You have now made it possible for MySQL to be restarted, but there’s one more thing
to do. To allow MySQL to be stopped, scroll down several more lines until you find
the section that starts with:
        "stop")
Below it you’ll see an indented line that reads:
                $0 stop-apache %
Just after this line, insert a new one that reads as follows:
                $0 stop-MySQL
Now you can press Ctrl-X to exit from edit mode, press the Y key when prompted to
save the changes, and then press Return to save the edited file.

[Previous](\Directory structure.md) [Next]
