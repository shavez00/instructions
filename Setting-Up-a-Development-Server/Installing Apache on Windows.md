There are several available WAMP servers.  For these exercises we're going to install each componet of our stack individually. The first componet is the Windows Operating System, which you already have installed.  The next componet is the Apache Web Server.

A Web server is a program that sends files to other computers.  Other computers request files from a web server using a web browser.  You're familiar with a web browser, it's how you're viewing this file right now.  When you type in a website, like Google.com, your computer sends a request to a web server at Google, requesting a file be sent back.  That file is a text file that sits on the web server the same way you have pictures on your phone or a word document on your computer.  Because of the format of that text file, your browser knows how to display it so that you see a website on your monitor.  That text files is called a web page and is coded using [HTML](http://www.html-5-tutorial.com/about-html.htm) (Hypertext Markup Language).  The web server uses a language called [HTTP](http://learn.onemonth.com/understanding-http-basics) (Hypertext Transfer Protocol) to talk to your browser.  That in a nut shell, is how the [Internet works](https://web.stanford.edu/class/msande91si/www-spr04/readings/week1/InternetWhitepaper.htm).

The Apache Web Server Project is an effort to develop and maintain an open-source HTTP server. The goal of this project is to provide a secure, efficient and extensible server that provides HTTP services in sync with the current HTTP standards.

You can download the latest version of Apache from the [Apache Haus Downloads website](http://www.apachehaus.com/cgi-bin/download.plx?dli=iVVU4NVRBNTTqd2aahUVyokVOpkVFVVchNTW410Z).

Once completed you should see the newly downloaded file in the bottom bar of your browser or in your download folder on your hard drive.  If you have trouble finding your newly downloaded file, just go to your windows search bar and type in "httpd" and you should be able to find it.  If you're not sure where the search bar is on Windows, go to Google and search for "Search bar" and your version of Windows and you should find some helpful websites that can help you find it.

Once downloaded, double click the downloaded file.  you will get a new windows like the one below:

{IMAGE}

Click the "Extract all files" option.  The ZIP extractor will select a default directory for you.  Change the default directory to "C:\" and click the Extract button. 

Now you need to install some software from Microsoft.  Go to the Microsoft site and download some software needed to run Apache.  Click [here](https://www.microsoft.com/en-us/download/details.aspx?id=48145) to download the software.  You'll see a red download button, click on the button and select the "vc_redist.x64.exe" file.  Download and install the software.

Congradulations, you've now created your first Web Server!

Now it's time to launch it.

Go to the Windows Start Button and in the search bar, input "CMD" to bring up the Command Prompt application.  Click cmd.exe to launch a window like the one below:

{IMAGE}

Change director to go to the root directory by typing "cd \" and then hit Enter.

You are now at the root directory of your computer.  From here we need to navigate to the Apache24 folder.

_If you don't see "Apache24" as one of the sub-directories in the next step, go back to your web browser or your download folder and double click the Apache Web Server file that you downloaded.  Make sure that when the file explorer window opens, and you click the "Extract all files" button that you change the "Files will be extracted to this folder:" text box to "C:\" and click Extract._

Type "dir" to bring up the list of sub-directories that exist under the root directory.  Look at the list of sub-directories and see if you can find the directory "Apache24".  

Feel free to play around by navigating to any of the other sub-directories and type "dir" to see a list of files and sub-directories that exist there.  Don't worry, you can get back to the root directory at any time by typing "cd \".  If you do look around your computer and you want to navigate back up one level, type "cd ..".  How many sub-directories deep into your directory structure can you wonder?

Once you're back to the root directory, type "cd Apache24" to navigate to the Apache sub-directory.  Type "dir" to bring up the list of files and directories that exist in the Apache directory.  Make note of some special sub-directories here.  You'll see a sub-directory called "conf", this will be where all of the files that configure how your webserver works are located.  You'll see a sub-directory called "htdocs", this is the instructions for the Apache Web Server.

Now we need to naviate to where Apache keeps it's [binary files](http://www.webopedia.com/TERM/B/binary_file.html), that's the actual program code that runs that makes a Web Server listen for browsers trying to connect to it.

Type "cd bin".

Now that you're in the binary directory type "dir" one last time.  In that long list of files, there's only one that's important at this time and that's the file named "httpd.exe".  This is the Apache [executable](http://searchsecurity.techtarget.com/definition/executable) that we need to run to start our web server.

Type "httpd".  It will look like nothing happened or that the computer has [hung](https://en.wikipedia.org/wiki/Hang_(computing)).  This isn't the case though, what's actually happened is that you've started your Apache Web Server.  Leave the terminal window open and go back to your web browser.

Type in "http://localhost" for the website you want to visit and you will see a page like below:

{IMAGE}

Congradulations!  You've now installed and run you're first web server.

[Previous](https://github.com/shavez00/instructions/blob/master/Setting-Up-a-Development-Server/What%20Is%20a%20WAMP-MAMP-LAMP.md) | [Next](https://github.com/shavez00/instructions/blob/master/Setting-Up-a-Development-Server/Storing%20information.md)
