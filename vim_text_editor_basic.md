# 1. vim text editor basic

1. `vim xxx`
1. edit: `i`
    1. input text
    1. delete: delete a character;
    1. use left, right, up, down arrow key for navigate input position; can use pageup, pagedown also;
1. save and quit: ecs
    1. `:q`: quit;
    1. `:q!`: don't save and quit;
    1. `:w`: save;
    1. `:wq`: save and quit;
1. visual: ecs
    1. yy: for copy 1 line; nff for copy n lines;
    1. p: for paste;
    1. dd: for delete 1 line; ndd for delete n lines;
    1. u: for undo;
    1. ctrl + r: redo;
    1. v: select character; then we can copy, delete, etc;
    1. shift + v: select lines;
    1. moving around
        - up, down, left, right arrow key
        - pageup, pagedown
        - "gg" go to begin of file, "shift + g" go to end of file
1. search: esc, then `/`;
    1. `/hello`: search hello string, likes in man command; 
        - n for next;
        - shift + n: for previous;
    1. replace: `:%s/hello/hi/g`;
        - ":s", means search and replace
        - "%", means match entire file
        - "hello" is what we want replace
        - "hi" is what we want replace to
        - "g", means match all in a line, default is match once in a line
