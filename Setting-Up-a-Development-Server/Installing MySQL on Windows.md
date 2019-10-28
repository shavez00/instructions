MySQL is the world’s most popular open-source database application and is commonly used with PHP. The MySQL software
comes with the database server (which stores the actual data), different client
applications (for interacting with the database server), and several utilities. .

Since the earliest releases, the MySQL developers have focused on performance, even
at the cost of a reduced feature set. To this day, the commitment to extraordinary speed
has not changed, although over time the formerly lacking capabilities have grown to
rival many of the commercial and open source competitors.

Although many open source projects enjoy an active user community, MySQL’s user
community might better be defined as hyperactive. For starters, there are thousands of open
source projects under way that depend upon MySQL as the back end for managing a
broad array of information, including server log files, e-mail, images, Web content,
help desk tickets, and gaming statistics. If you require advice or support, you can use
your favorite search engine to consult one of the hundreds of tutorials written regarding
every imaginable aspect of the software; browse MySQL’s gargantuan [manual](https://dev.mysql.com/doc/); or pose a
question in any of the high-traffic MySQL-specific newsgroups like [Stack Overflow](http://stackoverflow.com/questions/tagged/mysql). In fact, when researching
MySQL, the problem isn’t so much one of whether you’ll find what you’re looking for,
but where to begin!

We've now got Windows installed on our computer, Apache installed and running as our Web Server, it's now time to install MySQL as our Database Server.
You can download the MySQL software by navigating to the MySQL
Web site [Downloads section](https://dev.mysql.com/downloads/mysql/) and click on the blue download button.

{IMAGE}

Next click on the "Windows (x86, 32-bit), MSI Installer" download button.  It should show a download size of 1.7M.

{IMAGE}

The next page asks you to Login or Sign Up.  MySQL is managed by a company called Oracle.  An Oracle web account will allow you to recieve emails from Oracle with the latest developments for MySQL as well as their wide range of software and services.

If you choose to not Login or Sign Up, click the link "No thanks, just start my download." which appears below the Login and Sign Up buttons.

{IMAGE}

Once the download completes, double click the file that has been downloaded to your computer.  You will get a pop up window asking if you want to run the install program, click the "Run" button.  The MySQL installer will start and you will get another pop up window asking if you want to install MySQL, click "Yes".  The installer will run for a few minutes and you may get another pop up asking if the installer can make changes to your hard drive.  Click "Yes" again.

Now that the installer has started it will will ask if you want to download an upgrade to the installer.  In the pop up window, select "Yes".

After the latest version is downloaded and installed, you will recieve the license agreement window.  Select the "I accept the license terms" checkbox and then the "Next" button will become selectable.  Click the "Next" button.

{IMAGE}

The Choose Setup Type window will appear.  Use the default setting of "Developer Default" and click the "Next" button.

The next section is a bit more complex.

The next window is the Check Requirements window.  It is checking for software that MySQL needs in order to run successfully on your computer.  Click the "Execute" button at the bottom of the window and MySQL will attemp to locate and install the missing software.

There maybe some missing componets, but we won't need those.  A new pop up window asking if you are sure you want to proceed.  Click the "Yes" button.

You will be presented with a list of packages that are going to be downloaded and installed.  Click the "Execute" button to start the process.

Green checkmarks will appear next to each of the packages as their downloads complete.  Once they all have green checkmarks, click the "Next" button.

Now MySQL is download, it's time to configure our server.  Click "Next".  The configurator will ask you to select a TCP/IP port.  Use the default selection and click "Next".

It will now ask you to choose a Root password.  With servers you can have multiple accounts.  An account is the software and settings for that user.

For example, if you had an account on your computer, and you had an account for your little brother.  On your account you install your favorite game which is Mindcraft.  But your little brother doesn't like Mindcraft and doesn't install it using his account.  When you log into the computer using your user name and password, you will see Mindcraft installed and will be able to play it.  But if your little sister logs in your her user name and password, she won't see Mindcraft installed and won't be able to play it.  She also won't be able to use your Mindcraft game and mess up what you've created in Mindcraft.

This is why passwords are important.  If your little sister knows your password, she can log into your account and play your Mindcraft game, which you might not mind or you might hate.  But with computers, who uses your software and sees what you're doing should be up to the user.  That's how computers ensure each users privacy and security is by using accounts and passwords.

Whenever you are asked to create a password you should choose something easy for you to remember, but hard for someone else to guess.  Dates, names, places, and events are all good places to start when creating a password.  Combining these things together along with a symbol, can make an excellent password.  For example, if my birthday is January 7th, and I live in Portland, a good password is Jan7?Portland.  Hard for someone else to guess, but easy for me to remember.  Most people are tempted to write down their passwords as well.  While this is a sure fire way to make sure you don't forget your password, it's also a sure fire way for someone else to find it.  The best practice is pick a password that you can easily remember, and combine it with something else easy for you to remember with a symbol inbetween them.  That way your account is secure, and you won't run the risk of forgetting it.

There is a special type of account for each computer or server.  It's called [root](http://www.linfo.org/root.html) or [administrator](https://support.microsoft.com/en-us/help/14028/windows-7-how-log-on-as-an-administrator) (admin).  The root/administrator account has the ability to create or delete other accounts.  It decides who is allowed to do what on the computer or server.  All computers have to have a root account, someone has to have complete control over the system in order to create accounts for the users.  The root account also is the only account that can change someone's account password if they forget it.  But who resets the root account password if the person with the root account forgets their password?  Unfortuneately, no one.  There is no way to reset the root password if you lose or forget it.  For those two reasons, it's very important to set a very difficult password, but one that you as the holder of the root account, won't forget.

For the MySQL server installation, it's now time to set the root password.

There are now two text boxes.  The first asks "MySQL Root Password" and the second asks "Repeat Password".  You should select a password that is easy for you to remember, but hard for someone else to guess.  An example would be "my1stSQL!root" for both.

Next we need to create a user account.  Click the "Add User" button.

{IMAGE}

The Add User window will open.  Enter in your first name in the "Username" box, and select a password for your account.  Click the "OK" button and you will be taken back to the "Accounts and Roles" screen.  You have now give the MySQL root account a password and created a user account.  You can now click the "Next" button.

You will see the Windows Service window, click "Next".

You may see several [Plugin](https://en.wikipedia.org/wiki/Plug-in_(computing)) configuration screens.  Just click "Next" and on the next window "Execute".  The MySQL will go through a series of steps giving you updates as it runs through them.  As each step completes successfully you will see a green checkmark next to that step.  Once completed, you can click the "Finish" button.

Next the MySQL installer will check the configuration of your MySQL server.

Click "Next" on the next window.  

Then you will get the Connect to Server Window.  Click the "Check" button to check if your root account can log into the MySQL server.  Once that completes successfully, click the "Next" button.

{IMAGE}

In the next window, click Execute to apply the changes, then click the "Finish" button in the next window.

A third and final Product Configuration Window will appear.  Click "Next".

A confirmation that you have successfully installed MySQL will appear.  Click the "Finish" button.

Congradulations!  You have installed and configured your MySQL Database Server.

[Previous](https://github.com/shavez00/instructions/blob/master/Setting-Up-a-Development-Server/Storing%20information.md) | [Next](\What is PHP.md)
