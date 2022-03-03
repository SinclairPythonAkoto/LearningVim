# LEARNING VIM

In this folder you will find files that I have created using Vim.

As I learn, I will be creating new files and modifying old ones.

I will also create a list of Vim commands in this README file as I go along.

SOURCE: **https://www.youtube.com/watch?v=IiwGbcd8S7I**

Vim Cheet Sheet: **https://vim.rtorr.com**

### Inserting Data
To  make changes to an exsiting or new file you press `i` to activate the **INSERT** mode.
- Insert directly where cursor is - `i`
- Insert to the right of cursor - `a`
- Insert at the end of the line - `A`

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
- Move to TOP - `SHIFT` + `G` **CAPITAL G**
- Move to BOTTOM - `gg`
- Skip blocks of code DOWN - `}`
- Skip blocks of code UP - `{`
- Move cursor FORWARD to next word - `w`
- Move cursor FORWARD to next SPACE - `W`
- Move cursor BACKWARD to previous word - `b`
- Move cursor BACKWARD to previsuos SPACE - `B`
- Move cursor to designated line - `:20` **move cursor to line 20**
- Move cursor to beginning of line - `0`
- Move cursor to where text starts - `^`
- Move cursor to end of the line - `$`
- Move cursor to EXACT character within the line - `f` + *character* **Only works if character is in that line!**
- Move cursor to BEFORE character within the line - `t` + *character* **Only works if character is in that line!** 
- Toggle cursor to words of the same instance - `*` **This moves cursor to the next matching word** *This also prints out at the bottom of your Vim screen the word/characters your are searching for*
- Find the next instance of character within the line - `f` + *character* + `;` **This will keep searching for the given character in that line**

You can also put numbers in front these commands to move the cursor a certain amount of places:

- Move 50 lines down - `50` + `k`
- Move 20 lines up - `20` + `k`
- Move 10 code blocks up - `10` + `{`
- Moge 10 code blocks down - `10` + `}`

### Deleting Lines & Un-doing Them
- Delete a line - `dd`
- Revert changes - `u` **This reverts each deleted line made**
- Redo changes - `control` + `r`

### Copying & Pasting 
- Copy a line - `yy`
- Paste the copied line - `p` **This will paste the line below**
- Paste line above the cursor - `P`

When you delete a line it actually pastes it into the clipboard, where you can then paste the deleted line by using `p` or `SHIFT` + `P` **CAPITAL P**

You can also delete several lines of code by enetring the number follwed by `dd`
- Delete 10 lines - `10` + `dd`

### Using Visual The Line 
- Highlight your text via lines - `SHIFT` + `V` **CAPTIAL V**
- Highlight individual characters - `v`

When you have your text highleted you can then operate the same commands such as deleting code blocks, copying, pasting etc.

You can highlight sections of your text and then change it by pressing `c`
- Highlight & change by lines - `SHIFT` + `V` + `c`
- Highlight & change by characters - `SHIFT` + `v` + `c`

### Add New Line
- Add a new line below cursor - `o`
- Add a new line above cursor - `SHIFT` + `O` **CAPITAL O**

This create a new line and puts you into **INSERT** mode

### Changing Words
- Change a word - `cw`
- Change a wole line from point of cursor - `SHIFT` + `C`
- Change word(s) up until a specified character - `ct` + *character*

This removes the word where the cursor is and puts it into **INSERT** mode where you can then place the new text

### Deleting Words
- Delete a word - `dw`
- Delete rest of the line from point of cursor - `SHIFT` + `D` **CAPITAL D**
- Delete word(s) up until a specified character - `dt` + *character*
- Delete character where cursor is - `x`

This removes the word. The cursor needs to be at the beginning of the word, if it is placed in the middle or at the end it will only partially delete the chosen word.

### Lowercase / Uppercase Letters
- Change a letter to lowercase / uppercase - `~`

If the letter is a lowercase `~` will change it to an uppercase and vice versa

### Using The Period Command
- Re-doing the last previous command - `.`

This executes the last command you just done; so if you just deleted a line it will delete another line if you press `.` again.  Another example would be if you just renamed a piece of text, if you moved to another line it would repeat the same command - *but the key thing is that it would rename it to the exact same word that you had changed previously*.  **This is good when repeatign lines of code**
