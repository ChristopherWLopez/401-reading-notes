# command line reading notes

The use of arguments are very similar to what we do in js and that they follow there initial command options are used to modify there behavior of a command and often start with a ‘-‘.

A lot of names in bash are abbreviations .
It is great practice (since it is important to know where you are) to utilize the ‘pwd’ command to make sure you know where you are and that you are making the correct command in the correct location.
Alongside the pwd using ‘ls’ is perfect to check what is in your current directory.

‘Ls’ can take in arguments to fine tune this command. ‘-ls’ makes use of a ‘long listing’ command, this will show if the command the size of the file and alot of other specifics.

“Absolute directories specify a location (file directory) in relation to the root directory.” (Those begin with a forward slash.

“Relative paths” are found relative to where we currently are.

‘~’  is a shortcut to my home directory.
‘.’ Is us ‘..’ Is our parent directory.

I like the breakdown on the third section where they discuss “everything is a file” even though it seems obvious in retrospect it is kind of mind blowing to hear because all of this stuff feels very complicated and THAT kind of put it into perspective for me

You disclose what type of file you are working with after a full stop. This usually consists of 2-4 characters.

When we refer to a file (everything is a file) we are referring to a specific location ( because everything is a file). So the general rules of relative and absolute file paths is a way to get to our objects which it is a way to location, this is kind of cool to think, and really gives you a glimpse into the whole “value over reference” deal.

Spaces in names make the words two separate words… although valid this could really mess up what youre trying to do if you are not careful.

The use of the “manual” pages to help you seek what a command does is super helpful! I dont know why I overlooked this ! The fact that you can you look up the command and it will show you what it is and how to use is and its more nuanced details is pretty rad. I will totally be using this ALOT the us of the ‘/term’ to search for a term is also a big deal… this is look google but its already on your local machine.

## CHEAT-SHEET

### basic navigation

**pwd** : where you are in the system

**ls*path***: This performs a list of the current path.

**cd*path***: This is how you change into the given path. OR into your home directory.

**Path**: a desc. of where a file or directory is on thr file system.

**Absolute Path**:  One of the beginning from the root of the file system.

**Relative Path**: One relative to where you currently are in the system.

**~**: Used in paths as a reference to your home directory

**.**: Used in paths as a reference to your current directory (eg. ./bin )

### file manipulation

**mkdir<directoryname>**: creates a directory

**rmdir<directoryname>**: Remove a directory. (if empty).

**touch<filename>** :creates a blank file.

**cp<source> <destination>**: Copy the source file to the destination.

**mv <source> <destination>**: Move the source file to the destination.

**rm <path>**:Remove a file or directory.
Common options: -r -f.

### Manual pages

**man <command>**: View the man page for a command.

**man -k <search term>** : Search for man pages containing the search term.

**press q to exit man pages**.

[https://ryanstutorials.net/linuxtutorial/cheatsheet.php](info from ryanstutorials.net).