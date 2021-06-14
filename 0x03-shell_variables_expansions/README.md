# ALX SE program
## Shell Variable Expansions
All file start with #!/bin/bash
Assignement 1, Create a script that creates an alias of
+ name: ls
+ Value: rm *

alias ls="rm *"

Assignment 2, hello You

echo "hello $USER"

Assignment 3, 2-path

export PATH=$PATH:/action

Assignment 4, 3-path

echo $((`echo $PATH | grep -o ":/" | wc -l`+ 1))

Assignment 5, Global Variable

printenv

Assignment 6, Local Variables

set
