# 1. file and directory permission

### premission on file and directory

`ls -al` shows: `drwxr-xr-x  5  myuser mygroup  4096 Jun 20 09:40 java/`

1. `d`: for directory, dash for file;
1. `rwxr-xr-x`: 9 columns, 3 for user, 3 for group, last 3 for other user;
    1. `r` for read permission;
    1. `w` for write permission;
    1. `x` for execute permission;

### commands

1. `sudo`: use super privileges, example install packages we will use it, other methods is in root user, which is not recommend;
    1. sudo commands;
        1. chmod u-r java/
        1. ls -al java/: permission denied;
        1. so, we can use: `sudo ls -al java/`, input password;
    1. sudo su (short for sudo su root): run as root user;
1. chmod: change premission;
    - u means user, g means group, o means other user, a means all;
    - `chmod u-x java/`: it will be `rw-r-xr-x`
    - `chmod g+w java/`:  it will be `rw-rwxr-x`
    - `chmod -R o+w java/`: it will be `rw-rwxrwx`, and all it's subdirectories and files will have w permission for other user;
1. chown
    1. change the "/mnt/share" directory's owner and group from "root.vboxsf" to "j.j", by `"sudo chown -R j.j /mnt/share"`
        - "-R" means recursively
        - "j.j", first "j" is linux user, second is user group
1. gpasswd
    1. `gpasswd -a j vboxsf`, add user "j" to group "vboxsf"
        - "-a" means add


### others

1. discretionary access control (DAC)
    1. linux file and directory's permission
1. mandatory access control (mac): if you want control every operations on your system;
    1. selinux
    1. apparmor



