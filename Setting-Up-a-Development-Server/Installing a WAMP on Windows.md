There are several available WAMP servers, each offering slightly different configurations, for these exercises we're going to 
use Zend Server CE (where CE stands for Community Edition), because it’s free and is from the developers of PHP itself. You 
can download it from the [ZendCE website](http://tinyurl.com/zendce).
I recommend you always download the latest stable release (in this instance it’s 5.6.0
SP1 for Windows), which will be listed first in the download section of the web page.
The page should display the correct installer for your computer: Linux, Windows, or
OS X. You will be asked to log in before you download. You can click a link to get the
file without logging in or registering, but you’ll miss out on product update emails and
other news.

Once downloaded, run the installer to bring up the window in Figure 2-2.
Click Next and accept the license agreement that follows to move on to the “Setup
Type” screen (see Figure 2-3). Select the “Custom” option so that the MySQL server
can also be installed.


When the Custom Setup window appears, scroll down the list of options to the bottom
and ensure that both “phpMyAdmin” and “MySQL Server” are checked, as shown in
Figure 2-4. Then click Next.

On the following screen (see Figure 2-5), even if you already have an IIS web server
installed, I recommend that you choose to install the Apache web server because the
examples in this book are for Apache. Then click Next.
Accept the default values of 80 for the web server port and 10081 for the Zend server
interface port (see Figure 2-6), and click Next.
Once the ports have been assigned you will reach the screen in Figure 2-7, and you
should click Install to start the installation.

During installation some extra files may be downloaded, so it may take a few minutes
for the programs to get set up. When they are ready you will be notified that you can
start using the software by clicking Finish. When you do so your default browser will
be opened up with the page shown in Figure 2-8, where, to continue, you must check
the box to agree with the terms.
Now you are ready to set a password (see Figure 2-9). Make sure you choose one you
will remember, and click Next to proceed to the screen shown in Figure 2-10, where
you can now click Finish.

Finally your browser will show the Dashboard screen in Figure 2-11, which is the place
where you can administer the server.

You can return to this screen at any time by entering http://localhost:10081 into your
browser (or, if you entered a value other than 10081 for the Zend server interface port,
you can get to this screen by using that value after the colon instead).

[Next](\Testing the Installation.md) [Previous](\What Is a WAMP-MAMP-LAMP.md)
