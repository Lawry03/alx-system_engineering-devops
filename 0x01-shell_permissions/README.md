# Shell Permissions Scripting

## 0-iam_bstty
Using the (su - username) command, this script switches from the current user to 'betty.'

## 1-who_am_i
Using the (whoami) command, this script prints the effective username of the current 'user'.

## 2-groups
Using the (groups) command, this script prints all the groups the current 'user' is part of.

## 3-new_owner
Using the (chown betty hello) command, this script changes the owner of the file 'hello' to the user 'betty'.

## 4-empty
Using the (touch hello) command, this script creates an empty file called 'hello'.

## 5-execute
Using the (chmod u+x) command, this script adds execute permission to the owner of the file 'hello'.

## 6-multiple_permissions
Using the (chmod ug+x,o+r hello) command, this script adds execut permission to the user and group owner, and read permission to other user, the the file 'hello'.

## 7-everybody
Using the (chmod a+x hello) command, this script add execution permissions to the owner, group owner and other users to the 'hello' file.
