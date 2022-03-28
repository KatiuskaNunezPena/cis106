# Week Report 5

## Summary of Presentation : Managing files and directories


- **mkdir** :
This command mean "make directory" is use to create single or multiple directories.
Syntax: mkdir + directory name. For example, mkdir documents.
To create multiples directories in a single line use the following syntax: mkdir directory1 directory_2 directory3...
To create a directory with a parent directory at the same time .Use the following syntax: mkdir -p documents/photos.

Note: creating a directory with an existing name will give you an error.

- **touch**: 
This command is use to create files .

Syntax to create a file : `touch + Filesname`.
Example: `touch list`.

- To create several files in a single line use the following syntax:
`touch items_list.txt name_list`
- To create a file using relative path use the following syntax:
`touch ~/Documents/items_list.txt`
- To create a file using relative path use the following syntax(if your pwd is you home directory):
`touch Documents/items_list.txt`

**How to remove a file?**
-**rm**: this command is use to remove files.
syntax: `rm + file_name`

How to remove (empty/nonempty)directory or files?
- **rm -r**:
This command is use to remove non-empty directories.
syntax: `rm -r + directory_name`
example:`rm -r ~/Documents/photos`

   
- **rm -i**: this command remove a file and ask for confirmation before removal.
syntax:`rm -i + filename`
Example:`rm -i item_list`

- To remove all files inside a directory and ask for confirmation before removal:
syntax:`rm -I name/name/*`
Example:`rm -I Documents/photos/*`

- **rmdir**: 
This command is use to remove empty directories.
syntax:`rmdir Documents/photos`

**Move and rename directories and files**
- **mv**:
This command moves and renames directories.
Syntax to move a file : `mv + sources(where the file/directory is located) + destination (place where you want to move the file/irectory)`

  Example using relative path :`mv Documents/item_list Downloads/`

  Example moving multiple directories/files to a different directory`mv photos/ videos/ /media/student/flashdrive/`

  Syntax to rename a file: `mv + file_name.txt + filename2.txt`

  Example: `mv weeklyreport1.txt weeklyreport2`
  Example using absolute path: ` mv ~/Documents/cis106/weeklyreport/weeklyrepor1 /Documents/cis106/weeklyreport/weeklyrepor1 `

**Copy files and directories**

- **cp**: 
This command is use to copy files/directories from a source to another destination.
Syntax to copy files:`cp + files to copy + destination`
Example:`cp Downloads/img1.png Pictures/`
Syntax to copy multiple files in a single command:
`sudo cp -r text1.txt + text2.txt`
Example: `sudo cp -r homework1.txt weeklyreport.md`
Syntax to copy directories:`cp -r + directory to copy + destination`
Example:`cp -r ~ /Downloads/photos ~/Pictures` 

**Create hard link**
- **ln**:
This command is use to create a hard link.What is a hard link? are files that point to data on the hard drive.
Example: `ln file ~/Documents/fileml`


**Manual**
- **man**(manual):
This command displays a manual of any command that run on the terminal.
Syntax: `man + command_name`
Example: `man pwd`

  Syntax to open a specific man page:`man + number of the page + command_name`
Example: `man 5 passwd`

  Syntax to show the man page section:`man -f + command_name`
  Example: `man 5 passwd`

  Syntax to show all available pages of a command:`man -a + command_name`
  Example: `man -a pwd`

  Note: To exit the the man page press "q"


**Brace expansion**({}):
This is a feature of bash that allows to generate arbitrary string to use with commands.
 Example, `mkdir -p music/{jazz,rock}/{m3files,videos}new{1..3}`
Example removing multiple files: `rm -r {text1.tx,text2.txt,text3.txt}`