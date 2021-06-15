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

Assignment 13, Combination

Create a script that prints all possible combinations of two letters, except oo

+ Letters are lower cases, from a to z
+ One combination per line
+ The output should be alpha ordered, starting with aa
+ Do not print oo
+ our script file should contain maximum 64 characters

echo {a..z}{a..z} | tr " " "\n" | grep -v "oo"

Assignemt 14, Float

printf "%.2f" $NUM | sort

Assignment 15, Decimal to Hex


printf '%x\n' $DECIMAL


Assignment 16, Write a script that encodes and decodes text using the rot13 encryption. Assume ASCII

tr `echo {a..z} | tr -d ' '` `echo {n..z} $(echo {a..m}) | tr -d ' '` | tr `echo {A..Z} | tr -d ' '` `echo {N..Z} $(echo {A..M}) | tr -d ' '`
