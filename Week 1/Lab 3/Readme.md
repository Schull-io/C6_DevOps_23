# Linux Commands

## Aims and Objectives
Build familiarity with linux commands
Interact with remote repository

## Tasks

Step 1: Work with the commands,
Step 2: Do a screenshooot. 
Step 3: Atached proof in your local machine and push to the remote repo.




## Ls command

List all files in the current directory, including hidden files: ls -a
List all files in the current directory, including hidden files, and show their file sizes: ls -lh
List all files in the current directory sorted by modification time: ls -lt
List only directories in the current directory: ls -d */
List all files in the current directory, including hidden files, and display them in a long format with the owner's name: ls -l --show-control-chars --group-directories-first --author
List all files in the current directory and its subdirectories: ls -R
List all files in the curren t directory and its subdirectories, including hidden files: ls -R -a
List all files in the current directory and its subdirectories, sorted by file size: ls -R -S
List all files in the current directory and its subdirectories, showing their inode numbers: ls -R -i
List all files in the current directory and its subdirectories, showing the file type and permissions: ls -R -F


## Cp command
Copy a file from one directory to another: cp /path/to/source/file.txt /path/to/destination/
Copy multiple files at once: cp file1.txt file2.txt file3.txt /path/to/destination/
Copy a directory and its contents: cp -r /path/to/source/directory/ /path/to/destination/
Preserve the permissions of the original file when copying: cp -p /path/to/source/file.txt /path/to/destination/
Overwrite an existing file without prompting: cp -f /path/to/source/file.txt /path/to/destination/
Copy multiple files and rename them in the process: cp file1.txt file2.txt /path/to/destination/new_name1.txt new_name2.txt
Copy a file and create a backup of the original file: cp -b /path/to/source/file.txt /path/to/destination/
Copy a file and update the modified and access times of the copy: cp -p --preserve=timestamps /path/to/source/file.txt /path/to/destination/
Copy a file and only copy the part of the file between two specified offsets: cp --sparse=always --input-range=offset1:offset2 /path/to/source/file.txt /path/to/destination/
Copy a file and show progress while copying: cp -v /path/to/source/file.txt /path/to/destination/

## Mv command
Rename a file: mv old_name.txt new_name.txt
Move a file to a different directory: mv file.txt /path/to/destination/
Move multiple files to a different directory: mv file1.txt file2.txt file3.txt /path/to/destination/
Move a directory and its contents: mv -r /path/to/source/directory/ /path/to/destination/
Overwrite an existing file without prompting: mv -f /path/to/source/file.txt /path/to/destination/
Move a file and create a backup of the original file: mv -b /path/to/source/file.txt /path/to/destination/
Move a file and update the modified and access times of the copy: mv -p --preserve=timestamps /path/to/source/file.txt /path/to/destination/
Move a file and only copy the part of the file between two specified offsets: mv --sparse=always --input-range=offset1:offset2 /path/to/source/file.txt /path/to/destination/
Move a file and show progress while copying: mv -v /path/to/source/file.txt /path/to/destination/
Rename a file and change its file permissions at the same time: mv -v --preserve=mode /path/to/source/file.txt /path/to/destination/new_name.txt


## I/o redirection
Redirect the output of a command to a file: ls -l > file.txt
Append the output of a command to a file: ls -l >> file.txt
Redirect the output of a command to another command: ls -l | wc -l
Redirect the output and error messages of a command to a file: ls -l /non-existent-directory/ 2> error.txt
Redirect the error messages of a command to a file and display the output on the console: ls -l /non-existent-directory/ 2> error.txt 1>&2
Redirect the output and error messages of a command to separate files: ls -l /non-existent-directory/ 2> error.txt 1> output.txt
Redirect the output of a command to another command and also save it to a file: ls -l | tee file.txt | wc -l
Redirect the output of a command to another command and suppress the output to the console: ls -l | tee /dev/null | wc -l
Read a command's input from a file: sort < input.txt
Read a command's input from the output of another command: sort <(ls -l)


## Using pipes
Use grep to filter the output of ls: ls -l | grep ".txt"
Use awk to extract fields from the output of ls: ls -l | awk '{print $9}'
Use sed to modify the output of ls: ls -l | sed 's/^/ /'
Use uniq to remove duplicate lines from the output of ls: ls -l | uniq
Use head to display only the first few lines of the output of ls: ls -l | head -n 5
Using vi/vim to edit text files
Open a file in vi: vi file.txt
Navigate through the file using the arrow keys or h, j, k, l keys
Enter insert mode by pressing i and type or paste text into the file
Save the file and exit vi by pressing Esc, then typing :wq and pressing Enter
Open a new file in vi and save it with a different name: vi new_file.txt
Revert to a previous version of the file by pressing Esc, then typing :e! and pressing Enter
Search for a string in the file by pressing Esc, then typing /string and pressing Enter
Replace all occurrences of a string in the file by pressing Esc, then typing :%s/old_string/new_string/g and pressing Enter
Go to a specific line number by pressing Esc, then typing :line_number and pressing Enter
Split the window into multiple panes by pressing Ctrl + w followed by v or h to split vertically or horizontally, respectively. Navigate between panes using Ctrl + w followed by h, j, k, or l.
