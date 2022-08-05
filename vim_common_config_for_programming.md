# 1. vim common config for programming


~/.vimrc

```
" utf8 encoding
set fileencodings=utf-8

" when we input tab, vim will replace it with 4 space
set expandtab
set shiftround
set tabstop=4
set shiftwidth=4
set softtabstop=4

" indentation align
filetype indent on
" line number, turn off with "set nonumber"
set number

" syntax highlight
syntax enable
syntax on
```
