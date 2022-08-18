# NERDTree cheat sheet
[NERDTree](https://github.com/preservim/nerdtree) is a file system explore. It helps users to browse directory structure, find files and open them. Here is several tips to use NERDTree.

## Install NERDTree
Using Vim-Plug is highly recommended. After install Vim-Plug, Add this to `.vimrc`:
```
call plug#begin('~/.vim/plugged')
  Plug 'preservim/nerdtree'
call plug#end()
```
For more information about Vim-Plug, check out [here](https://github.com/junegunn/vim-plug).

## Keybinding to toggle NERDTree
Add this to `.vimrc` (vim version is `8.2`):
```
map <F10> :NERDTreeToggle<CR>
```
`F10` can be changed to other keys.

## Navigate between windows
NERDTree will open a window to show the directory tree.
```
-------------------------------------
|            |                       |
|            |                       |
| NERDTree   |        VIM            |
|            |                       |
|            |                       |
|            |                       |
-------------------------------------
```
Use `ctrl-w` + `w`(next),`h`(left) or`l` (right) to move between NERDTree and vim window.
For example, hit `control` and `w` simultaneously, and then hit `w` move to next window.

## Open files in split windows
Use `j`(up),`k`(down) to highlight the file in the NERDTree window and then hit `o` to open it.
```
-------------------------------------
|            |                       |
|            |                       |
| NERDTree   |        file1          |
|            |                       |
|            |                       |
|            |                       |
-------------------------------------
```

Navagate to the NERDTree and highlight a new file, hit `i` to open it in a horizontal split window.
```
-------------------------------------
|            |            |          |
|            |            |          |
| NERDTree   |    file1   |  file2   |
|            |            |          |
|            |            |          |
|            |            |          |
-------------------------------------
```
Navagate to the NERDTree and highlight a new file, hit `s` to open it in a vertical split window.

```
-------------------------------------
|            |            |          |
|            |            |   file2  |
| NERDTree   |    file1   |----------|
|            |            |          |
|            |            |   file3  |
|            |            |          |
-------------------------------------
```
Use `ctrl-w` + `w`(next window),`h`(left) or`l` (right),`j`(up),`k`(down)to move between NERDTree and vim window.
`ctrl-w` can be mapped to other [keys](#Keybinding-to-toggle-NERDTree).
