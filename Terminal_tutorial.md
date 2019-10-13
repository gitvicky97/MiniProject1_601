# Terminal Tutorial
* **What is Terminal?**

Terminal is a utility that allows you to interact with your Mac through the command line. Linux operating systems include similar tools, since both Linux and macOS are Unix-like OSes. The command line interface (CLI), or the language that you type into Terminal to interact with your Mac, is called **bash**. Everything we discuss below is a bash command.

* **Why Use the Terminal?**

Wasn't the whole point of graphical user interfaces to eliminate the need for a command line? Well, not really. There are still several reasons that you should learn how to use the Terminal if you are a developer, or even a user who cares about performance:

* Certain things simply cannot be done without the command line (especially as a developer). These include installing CocoaPods, using a git repository, and more

* You can easily make changes to your computer's settings which would be tedious or even impossible to do using the user interface only.

* The terminal is very flexible, and once you learn to use it, it is quite simple and straightforward.

* It is a very direct way of telling your computer what to do, whereas a GUI is akin to controlling the computer from a distance.

Those are just a few of the reasons that the Terminal is still a useful tool today. It's a practical and functional tool to improve and enhance your daily interactions with your computer.

# Getting Started

* Open **Terminal** 
Terminal is located in your **Applications** folder within a subfolder called **Utilities**. If you cannot find it, activate Spotlight search by pressing **Command-Spacebar** and search for **Terminal**. Once you have it open, you should see something which looks like this:
![Command Prompt](/images/Terminal.png)

# Basic Commands Cheat Sheet
Here is a list of some of the basic commands that you'll need to know in order to use the terminal effectively. This is a handy cheat sheet for the most important and most commonly used commands.

* **File Management**
    * **ls** 
    
    lists all of the contents in the current directory. This command comes in handy if you don't want to use the Finder to browse files—you can simply list them using this command in your Terminal.
    
    * **cd**
    
    **cd (directory name)** this command is used to change directories. If you write cd alone, you will move out of the current directory. After using ls (to see the directories), you can write the name of the directory you want to enter.
    
    * **mkdir** 
    
    this command Creates new folders in an instant with this command.
    **Example:** mkdir /Users/jdoe/Desktop/cool_stuff
    
    * **cp**
    
    **cp stands for copy.** This command is used to copy files or group of files or directory. It creates an exact image of a file on a disk with different file name. cp command require at least two filenames in its arguments.
    
     **For Example:**
     cp [OPTION] Source Destination
     cp [OPTION] Source Directory
     cp [OPTION] Source-1 Source-2 Source-3 Source-n Directory

     First and second syntax is used to copy Source file to Destination file or Directory.
     Third syntax is used to copy multiple Sources(files) to Directory.
    
    
    * **pwd**
    
    The basic usage, as is usually the case, is very easy. All you have to do is to run the 'pwd' command without any options, and you'll get the full path to the **current working directory in output.
    
    * **mv**
    
    this command helps us to quickly **move a file or folder into another folder using mv**. It works by simply changing the name of the path.

    The syntax is mv <old file path> <new file path>.

    **For example:**, mv /Users/jdoe/Documents/file1 /Users/jdoe/Desktop/file1 will move file1 from jdoe’s Documents to his Desktop.
    
    * **rm**
    
    This command will delete, immediately and without prejudice, any file you put in its path. Obviously, use it with extreme             caution. Unlike clicking **Empty Trash, rm** will not ask if you’re sure. It assumes you know what you’re doing.

     One thing to note about **rm** is that by default, it will only delete files, not folders. To delete folders, you must use the **-R** option, which stands for **recursive**.

     **Example**: rm -R /Users/jdoe/Desktop/cool_stuff
    
    * **history**
    
    All of our services are currently running on Linux. In Linux, there is a very useful command to show you all of the last commands that have been recently used. The command is simply called history, but can also be accessed by looking at your .bash_history in your home folder.
    
    
    Please check out the following interactive [Video](https://www.youtube.com/watch?v=5XgBd6rjuDQ) to understand how Terminal works! 

#    

* **File path in Linux**
    
    Files and folders on Linux are given names containing the usual components like the letters, numbers, and other characters on a keyboard. But when a file is inside a folder, or a folder is inside another folder, the / character shows the relationship between them. That’s why you often see files listed in the format **/usr/bin/python3 or /etc/os-release.** The forward slashes indicate that one item is stored inside of the item preceding it.

Every file and folder on a POSIX system can be expressed as a path. If I have the file **penguin.jpg** in the **Pictures** folder within my home directory, and my username is **seth**, then the file path can be expressed as **/home/seth/Pictures/penguin.jpg.

Most users interact primarily with their home directory, so the tilde (~) character is used as a shorthand. That fact means that I can express my example penguin picture as either **/home/seth/Pictures/penguin.jpg or as ~/Pictures/penguin.jpg.

* **Using the tab key to complete file paths**
   
   **Tab** is your friend

On a system famous for eschewing three-letter commands when two or even one-letter commands will do, rest assured that no seasoned POSIX user ever types out everything. In the Bash shell, the **Tab** key means autocomplete, and autocomplete never lies. For instance, to type the example **penguin.jpg** file’s location, you can start with:

$ ~/Pi

and then press the **Tab** key. As long as there is only one item starting with Pi, **the folder Pictures autocompletes for you.
      
      
* **Using up and down arrow for history**
   
   This command helps us to navigate through our history of commands which had been run previously.
   
For more Explanation of file path and navigation through files please check out [This link!](https://opensource.com/article/19/8/understanding-file-paths-linux)   
   
   
# Text editor Through Terminal  

* **What is the VI editor?**

The VI editor is the most popular and classic text editor in the Linux family. Below, are some reasons which make it a widely used editor –

   * It is available in almost all Linux Distributions
   * It works the same across different platforms and Distributions
   * It is user-friendly. Hence, millions of Linux users love it and use it for their editing needs

Nowadays, there are advanced versions of the vi editor available, and the most popular one is VIM which is Vi Improved. Some of the other ones are Elvis, Nvi, Nano, and Vile. It is wise to learn vi because it is feature-rich and offers endless possibilities to edit a file.

To work on VI editor, you need to understand its operation modes. They can be divided into two main parts.

1. **Command Mode**
2. **Insert Mode**

   * **Command Mode**
   
   1. The vi editor opens in this mode, and it only **understands commands**
   2. In this mode, you can, **move the cursor and cut, copy, paste the text**
   3. This mode also saves the changes you have made to the file
   4. **Commands are case sensitive.** You should use the right letter case.
   

   
   
   * **Insert Mode**
   
   1. This mode is for inserting text in the file.
   2. You can switch to the Insert mode from the command mode  **by pressing 'i' on the keyboard**
   3. Once you are in Insert mode, any key would be taken as an input for the file on which you are currently working.
   4. To return to the command mode and save the changes you have made you need to press the Esc key
   
         
To completely understand how to work with **vi text editor** Please go to the following **[link!]**(https://www.guru99.com/the-vi-editor.html)
For Interactive learning please watch the following **[Video]**(https://www.youtube.com/watch?v=pU2k776i2Zw&feature=youtu.be) to understand and get gist of vi text editor.



