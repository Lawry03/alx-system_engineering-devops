# Shell, I/O Redirections and filters

## 0-hello_world
Using the (echo "Hello, World") command, this script prints "Hello, World" followed bay a new line to the standard output.

## 1-confused_smiley
Using the (echo "\"(Ôo)'") command, this script displays a confused smiley. For special charecters press (Ctrl-v u charecter-unicode).

## 2-hellofile
Using the (cat /etc/passwd) command, this script displays the content of the /etc/passed file.

## 3-twofiles
Using the (cat /etc/passwd /etc/hosts), this script displays the content of both files, /etc/passwd and /etc/hosts.

## 4-lastlines
Using the (tail -n 10 /etc/passwd) command, this script displays the last 10 lines of /etc/passwd.

## 5-firstlines
Using the (head -10 /etc/passwd) command, this script displays the first 10 lines of /etc/passwd.

## 6-third_line
Using the (head -n 3 iacta | tail -n 1) command, this script displays the third line of the file iacta.

## 7-file
Using the (echo "Best School" > "\*\\\'\"Best School\"\'\\\*$\?\*\*\*\*\*:)") command, this script creates a file named exactly (   \*\\'"Best School"\'\\*$\?\*\*\*\*\*\*:)  )  containing the text Best School ending by a new line.

## 8-cwd_state
Usind the (ls -al > ls_cwd_content) command, this script writes into the file ls_cwd_content the result of the command ls -ls. If the ls_cwd_content file already exists, it is overwritten. If the file ls_cwd_content does not exist it is created.

## 9-duplicate_last_line
Using the (tail -1 iacta >> iacta) command, this script duplicates the last line of the file iacta.

## 10-no_more_js
Using the (find . -name "*.js" -type f -delete) command, this script deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfoldetrs.

## 11-directories
Using the (find . -type d ! -path . -print | wc -l) command , this script counts the number of directories and sub-directories in the current directory. Hidden directories are counted and the current and parent directories are not taken into account.

## 12-newest_file
Using the (ls -1t | head -10) command, this script displays the 10 newest files in the current directory. One file per line, sorted form newest to the oldest.

## 13-unique
Using the (sort | uniq -u) command, this script takes a list of words as input and prints only words that appear exactly once.
INPUT FORMAT : One line, One word.
OUTPUT FORMAT : One line, One word.
Words are sorted.

## 14-findthatword
Using the (grep root /etc/passwd) command, this script displays lines containing the pattern "root" from the file /etc/passwd.

## 15-countthatword
Using the (grep -c bin /etc/passwd) command, this script displays the number of lines that contain the pattern "bin" in the file /etc/passwd.

## 16-whatsnext
Using the (grep -A 3 root /etc/passwd) command, this script displays lines containing the pattern "root" and 3 lines after them in the file /etc/passwd.

## 17-hidethisword
Using the (grep -v bin /etc/passwd) command, this script displays all the lines in the file /etc/passwd that do not contain the pattern "bin".

## 18-letteronly
Using the (grep ^[[:alpha:]] /etc/ssh/sshd_config) command, this script displays all lines of the file /etc/ssh/sshd_config starting with a letter. Including capital letters.

## 19-AZ
Using the (tr "A" "Z" | tr "c" "e") command, this script replaces all characters A and c from input to z and e respectively.

## 20-hiago
Using the (tr -d "c" | tr -d "C") command, this script removes all letters c and C from input.

## 21-reverse
Using the (rev) command, this script reverse its input.

## 22-users_and_home
Using the (cut -d: -f1,6 /etc/passwd | sort) command, this script displays all users and their home directories, sorted by users.

## 100-empty_casks
Using the (find . -empty -printf "%f\n") command, this script finds all empty files and directories in the current directory and all sub-directories. Only the names of the files and directories are displayed. Hidden files are listed. One file name per line. The listing ends with a new line.

## 101-gifs
Using the (find -type f -name "*.gif" -printf "%f\n" | rev | cut -d '.' -f 2- | rev | LC_ALL=C sort -f) command, this script lists all the files with a .gif extension in the current directory and all its sub-directories. Hidden files are listed. Only regular files are listed (not directories). The names of the file are displayed without thier extensions. The files should be sorted by byte values, but case-insensitive. One file name per line. The listing ends with a new line.

## 102-acrostic
Using the (cut -c1 | paste -s | tr -d "[:blank:]") command, this script decodes acrostics that use the first letter of each line. The decode message ends with a new line.

## 103-the_biggest_fan
Using the (tail -n +2 | cut -f1 | sort | uniq -c | sort -nr -k 1,1 | cut -c 9- | head -11) command, this script parses wev servers logs in TSV format as input and displays the 11 hosts or IP addresses which did the most requests. Order by number of requests,most active host or IP at the top.
