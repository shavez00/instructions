The first thing to do at this point is verify that everything is working correctly. To do
this, you are going to try to display the default web page, which will have been saved
in the server’s document root folder (see Figure 2-12). Enter either of the following two
URLs into the address bar of your browser:
 http://localhost
 http://127.0.0.1

The word localhost is used in URLs to specify the local computer, which will also re-
spond to the IP address of 127.0.0.1, so you can use either method of calling up the
document root of your web server.

The document root is the directory that contains the main web documents for a domain.
This is the one that is entered when a basic URL without a path is typed into a browser,
such as http://yahoo.com, or, for your local server, http://localhost.
By default, Zend Server CE uses one of the following locations for this directory (the
former for 32-bit computers and the latter for 64-bit):
 C:/Program Files/Zend/Apache2/htdocs
 C:/Program Files (x86)/Zend/Apache2/htdocs

To ensure that you have everything correctly configured, you should now create the
obligatory “Hello World” file. Create a small HTML file along the following lines using
Windows Notepad or any other program or text editor (don’t use a rich word processor
such as Microsoft Word, unless you save as plain text):
<html>
  <head>
    <title>A quick test</title>
  </head>
  <body>
    Hello World!
  </body>
</html>
Once you have typed this in, save the file into the document root directory previously
discussed, using the filename test.htm—if you are using Notepad, make sure that the
“Save as type” box is changed from “Text Documents (*.txt)” to “All Files (*.*)”.
You can now call up this page in your browser by entering the following URL in its
address bar (see Figure 2-13):
 http://localhost/test.htm

You should now have had a trouble-free installation, resulting in a fully working
WAMP. But if you encountered any difficulties, check out the comprehensive docu-
mentation at http://tinyurl.com/zendcedocs, which should sort out your problem.

[Next] [Previous]()
