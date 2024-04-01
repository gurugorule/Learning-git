- Vim is Open-Source text editor, **Very Fast and Very Light** 
- Almost any [[Programming Language]] can be Edit/Run by using Vim
- To open file in Vim enter `vim file_name` in terminal 
## Vim has 3 Modes
#### Normal Mode : 
- To enter into Normal Mode press `Esc` key
- to Navigate between Text
	```
	h - left 
	j - down 
	k - up 
	l - right 
    ```
- Shortcuts keys to optimised experience with Vim 
	1. `u` - undo 
	2. `Ctrl + r` - redo 
	3. `x` - delete char
	4. `dd` - delete complete line and store it into paste buffer
	5. `p` - put / paste
	6. `gg` - go to beginning of the file
	7. `G` - go to end of the file 
	8. `Ctrl + ww` - switch between different split window 
	9. `%` to create file and `d` to create directory
***
#### Command Mode : 
- To enter into Command Mode press `Shift + ;` -> `:`
	1. `q` - quit / exit
	2. `w` - write / save 
	3. `wq` - save & exit  / write & quit
	4. `q!` - quit but don't save
	5. `x`  or `exit` - same as `wq` write & quit
	6. `!` - allow you to run bash command while using vim
	7. `r file_name` - read -> read the file_name and past the text into current buffer 
- `Buffer` is the small memory allocation which vim use to store text when file is not saved
	1. `e file_name` - to edit file_name buffer
	2. `bp` - buffer previous
	3. `bn` - buffer next
	4.  `bd` - buffer delete
	5. `badd file_name` - buffer add -> to add new file_name buffer 
	6. `enew` - to add new empty buffer
- To Search and replace text with new one
	- `%s/text/nex_text/g`
- To split vim window
	1. `split file_name` / `sp file_name` - Horizontal split between current_file and file_name
	2. `vsplit file_name`  / `vs file_name`- Vertical split between current_file and file_name
- Config tips
	1. to add line numbers `set number`
	2. to remover line numbers `set nonumber`
	3. to display file name at top bar `set title`
- To paste text copied from some were else (like Wikipedia or google)
	- Copy the text and in `COMMAND MODE` type `set paste`
	- Now you can paste the text via using `ctrl+shift+v` 
***
#### Visual Mode : 
- Press v in `NORMAL MODE` to enter into `VISUAL MODE` 
	1. in this mode you can select the text by Moving cursor with the help of ` h j k l` 
	2. `y` - to yank/copy the selected text
	3. `x` - to cut the selected text
	```
	then you can past the selecte text by pressing 'p' in NORMAL MODE
	```
  - To Sort the selected Lines of text in alphabetical order
	  1. press `:` in visual mode and type `sort ui`
	  

***
#### Insert Mode : 
- In this mode you can make changes/edits in the file 
- to enter in `INSERT MODE` press ' i ' in `NORMAL MODE`
- to get into `INSERT MODE` but at the end of line press ' A ' aka Append mode
**** 
Make a `.vimrc` file in `~` home directory -> add your config instruction into `.vimrc` file 
to customise vim [Vim customisation guide](https://www.freecodecamp.org/news/vimrc-configuration-guide-customize-your-vim-editor/)

`vim -o file_1 file_2` -> To open vim in horizontal split mode with file_1 and file_2
`vim -O file_1 file_2`-> To open vim in vertical split mode with file_1 and file_2
