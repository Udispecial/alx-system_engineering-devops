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

Assignment 7, create a script that create a new local variable

BETTY="Holberton"

Assignment 8, Create a script that creates a new global variable
+ Name: HOLBERTON
+ Value: Betty

export HOLBERTON="Betty"

Assignment 9, True Knowledge

echo $(($TRUEKNOWLEDGE + 128))

Assignment 10, Divide and rule

echo $(($POWER / $DIVIDE))

Assignment 11, Write a script that displays the result of BREATH to the power LOVE

+ BREATH and LOVE are environment variables

+ The script should display the result, followed by a new line

echo $(($BREATH**$LOVE))

Assignment 12, Write a script that converts a number from base 2 to base 10

echo $((2#$BINARY))