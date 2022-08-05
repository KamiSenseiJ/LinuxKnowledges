# 1. output redirection and pipe

1. `> file`: redirect ouput to file;
    1. `man man > man.txt`
1. `>> file`: append to end of file;
    1. `echo "hello, world." >> man.txt`
1. `command1 | command2`: pipe, connect input and output between commands;
    1. `cat man.txt | grep hello`, which equals `grep hello man.txt`
