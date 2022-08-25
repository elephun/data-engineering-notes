# Basic Command Line in Linux Terminal
## basics

`.` is the current working directory

Display current path:

`pwd`

Display the home directory from a terminal:

`cd ~` or `cd $HOME`

List files and directories:

`ls`

Use the cd command to change directories:

`cd directory/path`

Navigate up one directory:

`cd ..`

Touch to create a new file:

`touch file_name`

## copy file
Copy file example.txt file to `~/Documents` directory:

`cp example.txt ~/Documents`

Folders don't exist so use -r which means recursive and -v to see what has been copied:

`cp -r -v Documents ~/Mystuff`

Move files

`mv example.txt ~/Documents`

## new directory
Make a new directory:

`mkdir new_directory_name`

Make multiple directories at once using {}:

`mkdir {test1,test2,test3}`

## remove file
Remove file:

`rm file_to_remove.txt`


## searching files using find
Search for everything using find in current directory:

`find .`

Search for Directories only:

`find . -type d`

Search for Files
`find . -type f`

Finding a file name ending with `.txt`:

`find . -name "*.txt"`
## search within files using grep

Searching within files for patterns using grep. Searching for the word 'The' in the file haiku.txt:
This will return all 'The' and ones that contain 'The' like 'Thesis'

`grep The haiku.txt`

Searching for the stand alone word 'The'

`grep -w The haiku.txt`

Searching for the mulitple words 'The cat'

`grep -w "The cat" haiku.txt`

For more options, use the command:

`grep --help`