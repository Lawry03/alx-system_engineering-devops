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

## 8-James_Bond
Using the (chmod 007 hello) command, this script sets no permissions at all to the owner and group and allows for all permissions to the Other users.

## 9-John_Doe
Using the (chmod 753 hello) command, this script sets the mode of the file to -rwxr-x-wx.

## 10-mirror_permissions
Using the (chmod --reference=olleh hello) command, this script sets the mode of the file 'hello' the same as 'olleh's mode.

## 11-directories_permissions
Using the (chmod a+X *) command, this script adds execute permission to all subdirectories of the current directory for thegroup owner and all other users. Regular files will not be changed.

## 12-directory_permissions
Using the (mkdir -m751 my_dir) command, this sccript creates a directory called my_dir with permissions 751 in the working directory.

## 13-change_group
Using the (chgrp school hello) command, this script changes the group owner to 'school' for the file 'hello'.

## 100-change_owner_and_group
Using the (chown vincent:staff *) command, this script changes the owner to vincent and the group owner to staff for all the files and directories in the working directory.

## 101-symbolic_link_permissions
Using the (chown -h vincent:staff _hello) command, this script changes the owner and the group owner of _hello to vincent and staff respectively.

## 102-if_only
Using the (chown --from=guillaume betty hello) command, this script changes the owner of the file hello to betty only if it is owned by the user guillaume.

## 103-Star_Wars
Using the (telnet towel.blinkenlights.nl) command, this script will play the StarWars IV episode in the terminal.
