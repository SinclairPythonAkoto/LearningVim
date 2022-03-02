# LEARNING VIM

In this folder you will find files that I have created using Vim.

As I learn, I will be creating new files and modifying old ones.

I will also create a list of Vim commands in this README file as I go along.

SOURCE: **https://github.com/SinclairPythonAkoto/LearningVim.git**

Vim Cheet Sheet: **https://vim.rtorr.com**

### Inserting Data
To  make changes to an exsiting or new file you press `i` to activate the **Insert** mode.

### Exiting Vim
Don't be one of those who cannot exit Vim ! You can close Vim with the folling commands:
- Press `esc` then `:q`  - quit without saving (no changes)
- Press `esc` then `:q!` - quit without saving (after changes)
- Press `esc` then `:wq` - save changes and then quit
- Press `esc` then `:w`  - save chnages but keep file open

### Moving The Cursor 
The trackpad or mouse won't work in Vim! To move the cursor you  can use the navigation arrows, or do what real programmers do and use the keyboard to navigate through the content in your files.
- Move UP - `k`
- Move DOWN - `j`
- Move RIGHT - `l`
- Move LEFT - `h`
- Move to TOP - `SHIFT` + `g` **CAPITAL G**
- Move to BOTTOM - `gg`
- Skip blocks of code DOWN - `}`
- Skip blocks of code UP - `{`

You can also put numbers in front these commands to move the cursor a certain amount of places:

- Move 50 lines down - `50k`
- Move 20 lines up - `20k`
- Move 10 code blocks up - `10{`
- Moge 10 code blocks down - `10}`

### Deleting Lines & Un-doing Them
- Delete a line - `dd`
- Revert changes - `u` **This reverts each deleted line made**
- Redo changes - `control` + `r`

### Copying & Pasting 
- Copy a line - `yy`
- Paste the copied line - `p` **This will paste the line below**
- Paste line above the cursor - `P`

When you delete a line it actually pastes it into the clipboard, where you can then paste the deleted line by using `p` or `P`

You can also delete several lines of code by enetring the number follwed by `dd`
- Delete 10 lines - `10` + `dd`

