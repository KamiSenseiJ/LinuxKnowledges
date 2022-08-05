# 1. linux file and directory command


1. directory
    1. current directory: pwd;
    1. list files: ls; 
        - ll (alias ll="ls -al")
        - -a: means shows all files, include begin with `.` files;
        - -l: list common attributes;
    1. change current work directory: cd;
        - `cd xxx`: cd to xxx directory;
        - `cd .`: cd to current directory;
        - `cd ..`: cd to directory which above the current path;
        - `cd`: cd to home directory;
    1. create directory: mkdir (mkdir xxx)
1. file
    1. create: touch (touch xxx)
1. both
    1. copy
        - copy file: cp
            - `cp origin target`;
        - copy dirctory: cp -r
            - `cp -r origin target`;
    1. remove
        - file: rm; (rm xxx)
        - directory: (rm -r xxx)
    1. rename or move: mv (`mv origin target`)
1. wildcards: `*` (asterisk):  will match against none or many character;
    1. `ls *.java`
    1. `cp *.java tmp/`
    1. `mv *.java tmp/`
    1. `rm *.java`
