#ALX SE Program

week 3

##All program start with #!/bin/bash followed by your code

Assignment 1 

hello world program

echo 'Hello, World'\n

Assignment 2

Confused Smiley

echo "O.o"\

Assignment 3 Display the content of the /etc/passwd file

cat /etc/passwd

Assignment 4, display the content of /etc/passwd and /etc/hosts

cat /etc/passwd; cat /etc/hosts

Assignment 5, Display the last 10 lines of /etc/passwd

tail -n 10 /etc/passwd

assignment 6, Display the first 10 lines of /etc/passwd

head -10 /etc/passwd

Assignment 7, Write a script that displays the third line of the file iacta

cat iacta | head -3 | tail -1

Assignment 8, Creates a file named exactly \*\\'"Holberton School"\'\\*$\?\*\*\*\*\*:) containin
g the test Holberton School ending by a new line

echo "Holberton School" > \\\*\\\\"'\"Holberton School\"\\'"\\\\\*\$\\\?\\\*\\\*\\\*\\\*\\\*\:\)

Assignment  9, Write a script that writes into the file ls_cwd_content the result of the command ls -la. If the file ls_cwd_content already exists, it should be overwritten. If the file ls_cwd_content does not exist, create it

ls -la > ls_cwd_content

Assignment 10, Write a script that duplicate the last line of the file iacta

#!/bin/bash

tail -n 1 iacta >> iacta

Assignment 11, Write a script that deletes all the regular files (not the directories) with a .j
s extension that are present in the current directory and all its subfolders

find . -type f -name "*.js" -delete

Assignment 12, Write a script that counts the number of directories and sub-directories in the c
urrent directory

+The current and parent directories should not be taken into account

+Hidden directories should be counted
 
 find . -type d -not -name '.' | wc -l

Assignment 13, Create a script that displays the 10 newest files in the current directory

Requirements
+One file per line
+Sorted from the newest to the oldest

ls -t1 | head -n 10

Assignment 14,Create a script that takes a list of words as input and prints only words that appear exactly once

+Input format: One line, one word

+Outout format: One line one word

+Words should be sorted

sort | uniq -

Assignment 15, Display lines containing the pattern “root” from the file /etc/passwd

grep -i "root" /etc/passwd

Assignment 16, Display the number of lines that contain the pattern “bin” in the file /etc/passwd

grep -c -i "bin" /etc/passwd

Assignment 17, Display lines containing the pattern “root” and 3 lines after them in the file /etc/passwd

grep -i "root" -A 3 /etc/passwd
Assignment 18, Display all the lines in the file /etc/passwd that do not contain the pattern “bi
n”

grep -i -v "bin" /etc/passwd

Assignment 19, Display all lines of the file /etc/ssh/sshd_config starting with a letter

grep -i "^[a-z]" /etc/ssh/sshd_config

Assignment 20, Replace all characters A and c from input to Z and e respectively

tr "A" "Z" | tr "c" "e"

Assignment 21, Create a script that removes all letters c and C from input

tr -d "cC"

Assignment 22, Write a script that reverse its input

rev

Assignment 23, Write a script that displays all users and their home directories, sorted by users
+ Based on the the /etc/passwd file

cut -d ':' -f 1,6 /etc/passwd | sort

Assignment 24, Write a command that finds all empty files and directories in the current directory and all sub-directories

+ Only the names of the files and directories should be displayed (not the entire path)
+ Hidden files should be listed
+ One file name per line
+ The listing should end with a new line
+ You are not allowed to use basename, grep, egrep, fgrep or rgrep

find . -empty | rev | cut -d '/' -f 1 | rev

Assignment 25, A gif is worth ten thousand words

find -type f -name "*.gif" | rev | cut -d "/" -f 1 | cut -d '.' -f 2- | rev | LC_ALL=C sort -f

Assignment 26, Create a script that decodes acrostics that use the first letter of each line

find -type f -name "*.gif" | rev | cut -d "/" -f 1 | cut -d '.' -f 2- | rev | LC_ALL=C sort -f

Assignment 27, The biggest fan

tail -n +2 | cut -f -1 | sort -k 1 | uniq -c | sort -rnk 1 | head -n 11 | rev | cut -d ' ' -f -1 | rev
