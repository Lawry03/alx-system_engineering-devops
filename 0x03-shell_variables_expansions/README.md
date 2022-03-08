# Shell, Initialization files, Variabls and Expansions

## 0-alias
Using the (alias ls='rm *') command, this script creates an alias named "ls" and has a value "rm *".

## 1-hello_you
Using the (echo "hello $USER") command, this script prints 'hello user' , where user is the current Linux user.

## 2-path
Using the (export PATH="$PATH:/action") command, this script adds /action to the PATH. /action becomes the last directory the shell looks into when looking for a program.

## 3-paths
Using the (echo $PATH | tr ":" "\n" | wc -l) command, this script counts the number of directories in the PATH.

## 4-global_variables
Using the (env) command, this script lists enviroment variables.

## 5-local_variables
Using the (set) command, this script lists all local variables, environment variables, and functions.

## 6-create_local_variable
Using the (BEST="School") command, this script creates a new local variable named 'BEST' with the value of 'School'.

## 7-create_global_variable
Using the (export BEST="School") command, this script creates a new global variable named 'BEST' with the value of 'School'.

## 8-true_knowledge
Using the (echo $((128+TRUEKNOWLEDGE)) command, this script prints the result of the addition of 128 with the value stored in the enviroment variable called 'TRUEKNOWLEDGE'.

## 9-divide_and_rule
Using the (echo $(($POWER/$DIVIDE))) command, this script prints the result of 'POWER' divided by 'DIVIDE', followed by a new line. 'POWER' and 'DIVIDE' are enviroment variables.

## 10-love_exponent_breath
Using the (echo $(($BREATH**$LOVE))) command, this script displays the result of 'BREATH' to the power 'LOVE'. Both are enviroment variables. A new line follows after the result.

## 11-binary_to_decimal
Using the (echo $((2#$BINARY))) command, this script converts a number from  base 2 to base 10. The number in base 2 is stored in the enviroment variable 'BINARY'. The script displays the number in base 10, followed by a new line.

## 12-combinations
Using the (echo {a..z}{a..z} | tr ' ' '\n' | grep -v "oo") command, this script prints all possible combinations of two letters, except "00". The letters are lower cases, from 'a' to 'z'. One combination per line. Output in alpha order starting with 'aa'. With a maximum of 64 characters.

## 13-print_float
Using the (printf "%.2f\n" $NUM) command, this script prints a number with two decimal places, followed by a new line. The number is stored in the enviroment variable 'NUM'.

## 100-decimal_to_hexadecimal
Using the (printf '%x\n' $DECIMAL) command, this script converts a number from base 10 to base 16. The number in base 10 is stored in the enviroment variable 'DECIMAL'. The script displays the number in base 16, followed by a new line.

## 101-rot13
Using the (tr 'A-Za-z' 'N-ZA-Mn-za-m') command, this script encodes and decodes text using the 'rot13' encryption. Assuming ASCII.

## 102-odd
Using the (paste -d" " - - | cut -d " " -f 1) command, this script prints every other line from the input, starting with the first line.

## 103-water_and_stir
Using the (printf "%o\n" $(( $((5#$(echo $WATER | tr water 01234))) + $((5#$(echo $STIR |tr stir. 01234))) )) | tr 01234567 bestchol) command, this script adds the two numbers stored in the enviroment variables 'WATER' and 'STIR' and prints the result. 'WATER' is in base 'water'. 'STIR' is in base 'stir.' . The result is stored in base 'bestchol'.
