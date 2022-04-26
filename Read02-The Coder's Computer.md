
# The Coder's Computer  

Here is a summary of what to look for in a text editor.


## Terminal Cheatsheet  

A shell is a wrapper for the terminal, with a common shell being *Bash*. We are currently using ohmyzsh as our shell.  
**PWD** - print working directory - displays your current directory.  
**ls** - list - lists items within current directory. 

### File Paths

- Absolute - /home/user/documents  
- Relative - /documents  
- tilde(~) - shortcut for home path  
- dot(.) - reference to current directory  
- double dot(..) - reference to parent directory  

### Navigation

- cd - change directory (use tab to auto complete a partial destination name)
- file - use file\[filename] to determine the file type/extension
- case sensitivity - Linux is case sensitive. File1.txt and file.txt are different. So are file.TXT and file.txt.
- spaces in names - use escape character\[\\] before the space or put name in single quote \['file name']
- hidden files/folders - If name starts with a dot(.) then it is hidden. to find hidden use (ls -a) command

### Manual Pages

Use the command "man" plus the command your are inquiring about. (ex. man ls)  
Use keyword search with (man -k *keyword*)  
Use 'q' to quit manual pages  

### File Manipulation

- mkdir - make a directory(folder) at current directory
- mkdir -p - makes parent directory as needed (ex. mkdir -p folder1/folder2/folder3) would make folder1 and folder 2 if needed before making folder 3
- mkdir -v - displays text that shows the making of the directorys and filepath
- rmdir - removes a directory if it is empty (ls -a to show all hidden contents) (-p -v work as well)
- touch *filename.extension* - "creates" a blank file if it does not already exist. (remember case sensitivity for both name and extension)
- cp *source* *destination* - copies a file from the source path to the destination path (absolute or relative paths)
- cp -r - -r=recursive. copies all contents of source directory including subdirectories and subfiles to the destination path. Use caution. 
- mv *source* *destination* - moves a file from source path to destination path.
- mv as rename - if we move a file from and to the same directory we can rename i. (ex. mv /folder1/file1.txt /folder1/file2.txt. It will be renamed file2.txt)
- rm *filename* - removes a file (deleted)
- rmdir -r - removes directory and its contents. Use caution.

### Vi text editor

