---
name: Mohammed Chowdhury
semester: fall 23
course: cis106
---


## Final Assignment



### Question 1 


### ls 

Description: ls is used for listing the content of a given directory or the file/directory itself.
  
Syntax: ls + option + directory to list 


Example
ls - list the content of the present working directory.
ls -a - list all the files inside the current work directory including hidden files.
ls -lR  ~/Pictures


### mkdir

Description: mkdir is used for creating a single directory or multiple directories.

Syntax: mkdir + the name of the directory


Example
mkdir wallpapers -  create a directory in the present working directory
mkdir wallpapers / ocean - create a directory in a different directory using relative path
mkdir ~/wallpapers/forest - create a directory in a different directory using absolute path


### touch 

Description: touch is used for creating files 

syntax: touch filename


Example 
touch list -to create a file called list
touch list of colors.txt cars.txt drinks.txt - to create several files 
touch ~/Downloads/car.txt - to create a file using absolute path 

### mv

Description: mv moves and renames directories

syntax:mv + source + destination

example
mv Downloads/homework.pdf Documents/ - to move a file from a directory to another using absolute path
mv cars.txt mycars.txt – to rename a file
mv ~/Downlaods/cars.txt  ~ /Downlaods/mycars.txt – to rename a file using absolute path 


### cp 

Description: cp copies files/directories from a source to a destination

syntax: cp + files to copy + destination


example
cp Downloads/wallpapers.zip Pictures/ - to copy a file
cp -r  ~/Downloads/wallpapers ~/Pictures/ - to copy a directory with absolute path 
cp Downloads/wallpapers/* ~/pictures/ - to copy the content of a directory to another directory

### man 

Description: man displays the manual of commands

syntax: man command name

example 
man ls – excutable programs or shell commands 
man kill - system calls, which are system request that programs make to the kernel
man passwd – file formats and convention 


### cat 

Description: cat command is used for displaying the content of a file

syntax: cat + option + files to display 


example
cat todo.lst – display the content of a file located in the pwd
cat ~/Documents/todo.lst - display the content of a file using absolute path
cat -n ~/Documents/todo.md display the content of a file with line numbers 


### tac 

Description: tac command is used for displaying the content of a file in a reverser order 

syntax: tac + option + files to display 

example
tac cars.lst – display the content of a file located in the pwd
tac ~/Downloads/cars.lst - display the content of a file using absolute path 
tac -r -  This option will interpret the separator as a regular expression.


### head 

Description: Head command display the top N number of lined of a given file.

syntax: Head + option + files 

Example

head doc.txt. - Display the first 10 lines of a file
head -n 20 doc.txt - Display a specific number of lines from a file
head doc1.txt doc2.txt - Show the first part of multiple files


### tail 

Description: tail command display the last N number of lines of a given file

syntax: tail + option + file

example
tail file.txt - Display the last 10 lines of a file
tail -n 20 file.txt - Show the last 20 lines of a file
tail -f car.txt - Monitor changes in a file in real-time


### cut 

Description: cut command is used to extract a specific section of each lone of a file and display it to the screen

syntax: cut + option + files


example
cut -f1 doc.txt -  Extract the first field from a tab-separated file
cut -c3-6 doc.txt - Extract characters 3-6 from each line of a file
cut -d',' -f2 doc.csv - Extract fields using a different delimiter


### tr 

Description: tr command is used for translating or deleting characters from standard output 

syntax: standard output | tr + option set + set 

example 
cat doc.txt | tr -s “[:space:]” ‘ ‘ – translate tab into space
cat pic.txt | tr “[:space:]” ‘\t’ translate white space into tab
cat doc.txt | tr ‘.’ ‘,’  - translate one character to another 


### grep 

Description: grep is used to [search text in given file

syntax:grep + option + search criteria + files


example
grep 'word' file.txt - Search for a word in a file
grep -r 'pattern' directory/ ¬- Search recursively in a directory for a specific pattern
grep -v 'pattern' file.txt - Display lines not matching a pattern


### awk 

Description: awk is a scripting language used for processing and displaying text 

syntax: awk + option + {awk command} + file + file to save 

example 

awk -F: ‘{print $1}’ – print first filed of files  

$ awk '{print}' employee.txt - Awk prints every line of data from the specified file

$ awk '/use/ {print}' employee.txt - Print the lines which match the given pattern. 


### tree

Description: Tree  Displays directory structure in a tree-like format.

Syntax: tree options directory


Examples
Tree - Show directory structure with all files and folders
tree -L 2 - Display tree structure with specified depth
tree -a -  Include hidden files in the tree view 


### Questiion 2
**How to work with multiple terminals open?**

Open the first terminal then open another one and put them side by.

**How to work with manual pages?**

You can access these pages with the man command followed by the name of the command you want information on. For example, man ls will show the manual page for the ls command.

**How to parse (search) for specific words in the manual page**

To search for specific words in a man page, you can use the / key followed by the word you’re looking for. 

**How to redirect output (> and |)**

The > operator is used to redirect the output of a command to a file. For example, ls > file.txt will redirect the output of the ls command to file.txt. 

**How to append the output of a command to a file**

The >> operator is used to append the output of a command to a file. 

**How to use wildcards**

Wildcards are special characters that can represent other characters in commands. The most common wildcards are *, which represents any number of characters, and ?, which represents a single character10.

**For copying and moving multiple files at the same time**

To copy or move multiple files at once, you can list the files you want to copy or move, separated by spaces.

**How to use brace expansion**

Brace expansion {} is another feature of bash that allows you to generate arbitrary strings to use with commands. For example to create a N number of files use touch website {1..5}.html.


**For creating entire directory structures in a single command**

To create an entire directory structure in a single command, you can use the mkdir -p command followed by the directories you want to create, separated by slashes
