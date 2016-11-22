Before we launch into programming we need to take a quick detour and
talk about the windows command prompt, also know as the terminal window.

The command-line interface, sometimes referred to as the CLI, is a tool into which you can type text commands to perform specific tasks—in contrast to the mouse's pointing and clicking on menus and buttons. Since you can directly control the computer by typing, many tasks can be performed more quickly, and some tasks can be automated with special commands that loop through and perform the same action on many files—saving you, potentially, loads of time in the process.

Before Windows was created, the most common operating system that ran on computers was DOS. DOS stands for Disk Operating System and was what you would use if you had started your computer much like you do today with Windows. The difference was that DOS was not a graphical operating system but rather purely textual. That meant in order to run programs or manipulate the operating system you had to manually type in commands. When Windows was first created it was actually a graphical user interface that was created in order to make using the DOS operating system easier for a novice user. As time went on and newer versions of Windows were developed DOS was finally phased out with Windows ME. Though the newer operating systems do not run on DOS, they do have something called the command prompt, which has a similar appearance to DOS. In this tutorial we will cover the basic commands and usage of the command prompt so that you feel comfortable in using this resource.

When people refer to the command prompt they may we refer to it in different ways. They may refer to it as a shell, console window, a command prompt, a cmd prompt, or even dos. In order to enter the command prompt you need to run a program that is dependent on your operating system. Below we list the programs that you need to run to enter a command prompt based on the version of Windows you are running.
 
Step 1: Click on the Start Menu

Step 2: Click on the Run option

Step 3: Type the appropriate command in the Open: field. For example if we are using Windows XP we would type cmd.exe.

Step 4: Click on the OK button

After following these steps you will be presented with a window that look similar to Figure 1 below.

The command prompt is simply a window that by default displays the current directory, or in windows term a folder, that you are in and has a blinking cursor ready for you to type your commands. For example in Figure 1 above you can see that it says C:\WINDOWS>. The C:\WINDOWS> is the prompt and it tells me that I am currently in the c:\windows directory. If I was in the directory c:\program files\directory the prompt would instead look like this: C:\PROGRAM FILES\DIRECTORY>.

To use the command prompt you would type in the commands and instructions you want and then press enter. In the next section we will discuss some useful commands and how to see all available built in commands for the command prompt.

The Command Prompt is a command line interpreter application available in most Windows operating systems.

Command Prompt is used to execute entered commands. Most of those commands are used to automate tasks via scripts and batch files, perform advanced administrative functions, and troubleshoot and solve certain kinds of Windows issues.

Command Prompt is officially called Windows Command Processor but is also sometimes called the command shell or by its filename cmd.exe.

The command.com or cmd.exe programs have built in commands that are very useful. Below I have outlined some of the more important commands and further instruction on how to find information on all the available commands.

The Help command - This command will list all the commands built into the command prompt. If you would like further information about a particular command you can type help commandname. For example help cd will give you more detailed information on a command. For all commands you can also type the command name followed by a /? to see help on the command. For example, cd /?

The Exit command - This command will close the command prompt. Simply type exit and press enter and the command prompt will close.

The CD command - This command allows you to change your current directory or see what directory you are currently in. To use the CD command you would type cd directoryname and press enter. This would then change the directory you are currently in to the one specified. When using the cd command you must remember how paths work in Windows. A path to a file is always the root directory, which is symbolized by the \ symbol, followed by the directories underneath it. For example the file notepad.exe which is located in c:\windows\system32 would have a path as follows \windows\system32\notepad.exe. If you want to change to a directory that is currently in your current directory you do not need the full path, but can just type cd directoryname and press enter. For example if you are in a directory called c:\test, and there were three directories in that the test directory called A, B, and C, you could just type cd a and press enter. You would then be in the c:\test\a. If on the other hand you wanted to change your directory to the c:\windows\system32 directory, you would have to type cd \windows\system and press enter.

The DIR command - This command will list the files and directories contained in your current directory, if used without an argument, or the directory you specify as an argument. To use the command you would just type dir and press enter and you will see a listing of the current files in the directory you are in, including information about their file sizes, date and time they were last written to. The command will also show how much space the files in the directory are using and the total amount of free disk space available on the current hard drive. If I typed dir \test I would see the contents of the c:\test directory as shown in Figure 2 below.


If you examine the screen above you will see a listing of the directory. The first 2 columns are the date and time of the last write to that file. Followed by whether or not the particular entry is a directory or a file, then the size of the file, and finally the name of the file. You may have noticed that there are two directories named . and .., which have special meaning in operating systems. The . stands for the current directory and the .. stands for the previous directory in the path. In the example above, .. stands for c:\windows.

Also note for many commands you can use the * symbol which stands for wildcard. With this in mind, typing dir *.txt will only list those files that end with .txt.

The Copy command - This command allows you to copy files from one location to another. To use this command you would type
copy filetocopy copiedfile. For example if you have the file c:\test\test.txt and would like to copy it to c:\windows\test.txt you would type
copy c:\test\test.txt c:\windows\test.txt and press enter. If the copy is successful it will tell you so and give you back the prompt. If you are copying within the same directory you do not have to use the path. Here are some examples and what they would do:

copy test.txt test.bak	Copies the test.txt file to a new file called test.bak in the same directory
copy test.txt \windows	Copies the test.txt file to the \windows directory.
copy * \windows	Copies all the files in the current directory to the \windows directory.
The Move command - This command allows you to move a file from one location to another. Examples are below:

move test.txt test.bak	Moves the test.txt file to a new file renaming it to test.bak in the same directory.
move test.txt \windows	Moves the test.txt file to the \windows directory.
move * \windows	Moves all the files in the current directory to the \windows directory.
At this point you should use the help command to learn about the other available commands.

[Previous](\Intro.md) [Next] (\Directory structure.md)
