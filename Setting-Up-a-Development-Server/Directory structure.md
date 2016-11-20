In the last section we learned about the windows terminal, which will be important for working with our newly installed WAMP stack, but before we continue working with the WAMP stack, we need to learn about the file system and directory structure.

The directory structure in the terminal window is just like the one in Windows.
The drive C represents the root directory written as C:\ nested directories are called Sub-directories.
Everything looks exactly like a tree except the roots are at the top !!

The directory that hosts subdirectories is called Parent directory.
When listing directory content using DIR, (..) refers to Parent directory
so if we're at C:\WINDOWS\Desktop> (.) refers to Desktop and (..) refers
to WINDOWS. If you're wondering whether the dots are useful, the answer is a straight YES.
The dots are used to navigate or explore the directories.

Suppose you want to switch to WINDOWS directory and apply the DIR command, you can use the Change Directory command CD, just type CD.. to go to WINDOWS directory. 
The CD command is very useful when you want to navigate in DOS. To go back to Desktop type CD desktop.

If you follow the tree structure - with Root directory C at the top -
typing cd.. while in Desktop will move you one level up.
If you continue to type cd.. you will eventually reach the top of the tree, the root directory.

If you type cd.. after you reach the root directory you will get:

C:\>cd..
Invalid directory 
