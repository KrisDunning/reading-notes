[Return to main page](https://KrisDunning.github.io/reading-notes/)

# Terminal Notes Cheatsheet  

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

- vi *file* - opens the file for text editing directly in terminal
- insert/edit - press i when in vi to insert content into the open file. press esc key to leave insert mode and enter edit mode (move,copy,save,replace, etc)
- edit mode commands
  - ZZ - save and exit
  - :q! - discard all changes, since the last save, and exit
  - :w - save file but don't exit
  - :wq - again, save and exit
- cat *file1* *file2*- short for concactenate or join two files. but easy way to view a file if only use one file
- CTRL+C - the terminal universal cancel/quit command
- less *file* - allows user to use arrow keys to navigate viewing of a file. <spacebar> to move a whole page or \<b> to go back a page. \<q> to quit.
- Navigation within Vi insert mode
  - Arrow keys - move the cursor around
  - j, k, h, l - move the cursor down, up, left and right (similar to the arrow keys)
  - ^ (caret) - move cursor to beginning of current line
  - $ - move cursor to end of the current line
  - nG - move to the nth line (eg 5G moves to 5th line)
  - G - move to the last line
  - w - move to the beginning of the next word
  - nw - move forward n word (eg 2w moves two words forwards)
  - b - move to the beginning of the previous word
  - nb - move back n word
  - { - move backward one paragraph
  - } - move forward one paragraph
- :set nu - typed in edit mode allows line numbers to be visible
- Delete/Undo in Vi
  - x - delete a single character
  - nx - delete n characters (eg 5x deletes five characters)
  - dd - delete the current line
  - dn - d followed by a movement command. Delete to where the movement command would have taken you. (eg d5w means delete 5 words)
  - u - Undo the last action (you may keep pressing u to keep undoing)
  - U (Note: capital) - Undo all changes to the current line

### Wildcards

Baby steps towards REGEX...

- asterisk(*) - asterisk is used to include all. (ex. ls b* will list all content that starts with a b)
- question mark(?) - question mark is used to represent a single character (ex. ls ?b* will return all files that have the 2nd letter of b)
- range ([]) - includes a range of items. (ex. ls *[0-9]* will return files that include any number.
- caret(^) - inverts the range to exclude items (ex. ls *^[0-9]* will excludes any files that include a number.
  
### Permissions

Three types of permissions
  - r - read
  - w - write
  - x - execute  
  
Three types of ownership
  - owner - the single person responsible for ownership of the file
  - group - every file belongs to a single group
  - others - everyone else who is not owner or in the group
  
To view permissions we use the long view of list (ls -l *filename*)
  Example: ls -l myfile.txt 
  returns: -rwxr----x etcetcetcetcetcetc
  The first character is filetype (- is file) (d is directory)
  The next 3 are the owner permissions (r=read w=write x=execute)
  The next 3 are the groups permissions (r=read -=no write permission -=no execute permission)
  The last 3 are the others permissions (-=no read -=no write permissions x=execute permission)
  
To change permission we use *chmod* [permission][path]
  - The permission options are "ugoa", or user-group-others-all
  - Then add a plus(+) to include permission or a dash(-) to remove permission
  - example: chmod a+rwe picture.png will give all users read, write and execute permissions

  *********
  
[Return to main page](https://KrisDunning.github.io/reading-notes/)