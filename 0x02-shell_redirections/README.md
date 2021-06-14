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
Assignment 8, Creates a file named exactly \*\\'"Holberton School"\'\\*$\?\*\*\*\*\*:) containing the test Holberton School ending by a new line
echo "Holberton School" > \\\*\\\\"'\"Holberton School\"\\'"\\\\\*\$\\\?\\\*\\\*\\\*\\\*\\\*\:\)
Assignment  9, Write a script that writes into the file ls_cwd_content the result of the command ls -la. If the file ls_cwd_content already exists, it should be overwritten. If the file ls_cwd_content does not exist, create it
ls -la > ls_cwd_content
Assignment 10, Write a script that duplicate the last line of the file iacta
#!/bin/bash
tail -n 1 iacta >> iacta
Assignment 11, Write a script that deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders
find . -type f -name "*.js" -delete
Assignment 12, Write a script that counts the number of directories and sub-directories in the current directory
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
Assignment 16 Display the number of lines that contain the pattern “bin” in the file /etc/passwd
grep -c -i "bin" /etc/passwd
