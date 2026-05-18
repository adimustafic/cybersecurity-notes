# Windows Fundamentals

**Windows** is the most-used OS for personal or work computers in the world. It is used on millions on devices daily. It's GUI (Graphical User Interface) is intuitive and easy to understand, so even beginners can quickly adapt to it. It allows customization, so the user can set it to their liking. There are two main types of window operating system's:

- Windows client
- Windows server

The file system Windows uses is called **NTFS** _(New Technology File System)_. On NTFS volumes, you can set permissions that grant or deny access to files and folders.

The permissions are:

- Full control
- Modify
- Read & Execute
- List folder contents
- Read
- Write

To see permissions of a file or a folder you would go to `Properties`, then click on `Security` tab and in the panel named `Group or user names:` you can see which user has which permissions.

### Windows location

By default, the Windows OS is located on `C:\` drive in the folder called `windows`, but it can be set, or installed on a different drive under the different name during partiotioning phase of system installation. This is where environment variables, more specifically system environment variables, come into play. The system environment variable for the Windows directory is `%windir%`. The most important part of the `windows` folder is another folder called `system32` which houses most of the important files that are critical for the operating system. Accidentally deleting any files or folders within System32 can render the Windows OS inoperational.

### User accounts

User accounts in Windows can be of 2 types:

1. Administrator account - make changes to the system: add users, delete users, modify groups, modify settings on the system, etc.
2. Standard user account - make changes to folders/files attributed to the user & can't perform system-level changes, such as install programs.

The location for each user account is `C:\Users`.
To get an overview of available groups and users we can open a program called `Run` and type in `lusrmgr.msc` which opens a control panel for groups and users.

### Settings

To take full "control" of the system we use 2 different programs. First, and most widely used is just called `Settings`, and it was introduced in Windows 8. It is catered for beginner and is mainstreamed. While on the other hand, an older way to access all of your settings on a Windows OS we used the `Control Panel`, which has a more detailed and complex menu, but I dare to say it is the more powerful of the two. Or at least it was. In today's Windows OS the two are interconnected and each has it's uses.

### Troubleshooting

If, or more likely when we come across some problems with Windows, we mainly use a tool called `msconfig` for figuring out and solving the problem. Tp access it, we just type `msconfig` into the search bar on `Start` menu, and open `System configuration` panel. Other tool we can use for diagnosis is `Event Viewer`. It shows all events sorted by the time they happened, and it logs their summaries.

For managing most of our computers we can use `Computer Managment` tool, which is accessed by typing `compmgmt` into the search bar in the Start menu.

To get a comprehensive view of your hardware, system components, and software environment we use the `msinfo32` tool.

### **CMD**

Although Windows is primarily centered around it's GUI, it also comes with it's own CLI, called `CMD` (Command prompt).
Some of the most basic **cmd** commands are:
```cmd
hostname - output computer's name
whoami - output the name of the logged-in user
ipconfig - show network address settings
/? - open a command manual, f.e. ipconfig /?
cls - clear command prompt
netstat - display protocol statistics and current TCP/IP network connections
net - manage network resources
help - used when there is no manual available, f.e. net help
