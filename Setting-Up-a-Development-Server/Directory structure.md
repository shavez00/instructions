In the last section we learned about the windows terminal, which will be important for working with our newly installed WAMP stack, but before we continue working with the WAMP stack, we need to learn about the file system and directory structure.

In computing, a directory structure is the way an operating system's file system and its files are displayed to the user. Files are typically displayed in a hierarchical tree structure.

In Windows the root directory is "drive:\", for example, the root directory is usually "C:\". The directory separator is usually a "\", but the operating system also internally recognizes a "/". Physical and virtual drives are named by a drive letter, as opposed to being combined as one.[1] This means that there is no "formal" root directory, but rather that there are independent root directories on each drive. However, it is possible to combine two drives into one virtual drive letter, by setting a hard drive into a RAID setting of 0.[2]

In a computer file system the root directory is the first or top-most directory in a hierarchy. It can be likened to the trunk of a tree, as the starting point where all branches originate from. It is the directory on top of which all other directories are branches off or.  In Windows this is "C:\".

To use the example of a physical file cabinet, The file cabinet is the root directory and each of the sub-directories under root would be a drawer inside of the filing cabinet. In Windows, files can be placed inside the root directory, as well as in its sub-directories. One may envision this as placing paper files on top of the filing cabinet, or into any of the drawers within the filing cabinet.  As in real life, it's not a good idea to place papers on top of the filing cabinet, it's also not a good idea to put files in the root directory of your computer's file system.

Below is an example of what a directory path would look like in a Windows command line path

In the above example, C: is the drive letter and the current directory is System32, which is a subdirectory of the Windows directory.

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

[Previous](\Terminal window.md) [Next](\Configuring MySQL.md)
