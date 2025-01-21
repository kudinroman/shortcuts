## Navigation

| Shortcut | Explanation                                                         |
| -------- | ------------------------------------------------------------------- |
| %        | Jump to the matching parenthesis, bracket, or brace (:h matchpairs) |
| M        | Move to middle of screen                                            |
| ^        | Jump to the first non-blank character of the line                   |
| Ctrl + e | Move screen down one line (without moving cursor)                   |
| Ctrl + y | Move screen up one line (without moving cursor)                     |
| Ctrl + f | Move forward one full screen                                        |
| Ctrl + b | Move back one full screen                                           |
| Ctrl + d | Move forward 1/2 a screen                                           |
| Ctrl + u | Move back 1/2 a screen                                              |

## Editing Text

| Shortcut       | Explanation                                                                                              |
| -------------- | -------------------------------------------------------------------------------------------------------- |
| a              | Enter Insert mode after the cursor                                                                       |
| I              | Enter Insert mode at the beginning of the line                                                           |
| A              | Enter Insert mode at the end of the line                                                                 |
| o              | Insert a new line below the current line                                                                 |
| O              | Insert a new line above the current line                                                                 |
| ciw            | Change inside word (delete the word under the cursor and enter Insert mode)                              |
| cw             | Change (replace) to the nd of the word                                                                   |
| caw            | Change around word (delete the word under the cursor including surrounding spaces and enter Insert mode) |
| cit            | Change inside tag (useful for HTML/XML editing)                                                          |
| cib            | Change inside block (delete the content inside parentheses or braces and enter Insert mode)              |
| gU             | Convert selected text to uppercase                                                                       |
| gu             | Convert selected text to lowercase                                                                       |
| J              | Join line below to the current one with one space in between                                             |
| gJ             | Join line below to the current one without space in between                                              |
| cc or S        | Change (replace) entire line                                                                             |
| c$ or C        | Change (replace) to the end of the line                                                                  |
| s              | Delete character and substitute text                                                                     |
| xp             | Transpose two letters (delte and paste)                                                                  |
| yw             | Yank (copy) the characters of the word from the cursor position to the start of the next word            |
| yiw            | Yank (copy) word under the cursor                                                                        |
| yaw            | Yank (copy) word under the cursor and the space after or before it                                       |
| y$ or Y        | Yank (copy) to the end of line                                                                           |
| dw             | Delete (cut) the characters of the word from the cursor position to the start ot the next word           |
| diw            | Delete (cut) word under the cursor                                                                       |
| daw            | Delete (cut) word under the cursor and the space after ro before it                                      |
| g/{pattern}/d  | Delete lines starting from 3 to 5                                                                        |
| g!/{pattern}/d | Delete all lines not containing pattern                                                                  |
| d$ or D        | Delete (cut) to the end of the line                                                                      |
| x              | Delete (cut) character                                                                                   |
| >>             | Indent (move right) line one shiftwidth                                                                  |
| <<             | De-indent (move left) line one shiftwidth                                                                |
| >%             | Indent a block with () or {} (cursor on brace)                                                           |
| <%             | De-indent a block with () or {} (cursor on brace)                                                        |
| >ib            | Indent inner block with ()                                                                               |
| >at            | Indent inner block with <>                                                                               |
| 3==            | Re-indent 3 lines                                                                                        |
| =%             | Re-indent a block with () or {} (cursor on brace)                                                        |
| =iB            | Re-indent inner block with {}                                                                            |
| dt             | Delete till                                                                                              |

## Visual mode

| Shortcut | Explanation                      |
| -------- | -------------------------------- |
| v        | Start visual mode                |
| V        | Start linewise visual mode       |
| Ctlr+V   | Start visual block mode          |
| o        | Move to other end of marked area |
| O        | Move to other corner of block    |
| aw       | Mark a word                      |
| ab       | Mark a block with ()             |
| aB       | Mark a block with {}             |
| at       | Mark a block with <> tags        |
| ib       | Inner block with ()              |
| iB       | Inner block with {}              |
| it       | Inner block with <> tags         |
| ~        | Switch case                      |

## File Management

| Shortcut    | Explanation             |
| ----------- | ----------------------- |
| :e filename | Open a file for editing |

## Search and Replace

| Shortcut                        | Explanation                                                                                   |
| ------------------------------- | --------------------------------------------------------------------------------------------- |
| /                               | Search forward for a pattern                                                                  |
| ?                               | Search backward for a pattern                                                                 |
| :%s/pattern/replacement/g       | Replace all occurrences of 'pattern' with 'replacement' in the entire file                    |
| :s/pattern/replacement/gc       | Replace all occurrences of 'pattern' with 'replacement' in the current line with confirmation |
| :bufdo %s/pattern/replacement/g | Replace 'pattern' with 'replacement' in all open buffers                                      |
| :g/pattern/d                    | Delete all lines containing 'pattern'                                                         |

## Splits and Tabs

| Shortcut   | Explanation                   |
| ---------- | ----------------------------- |
| :sp        | Split the window horizontally |
| :vsp       | Split the window vertically   |
| :tabnew    | Create a new tab              |
| :tabclose  | Close the current tab         |
| :tabn      | Go to the next tab            |
| :tabp      | Go to the preious tab         |
| Ctrl + w s | Split the window horizontally |
| Ctrl + w v | Split the window vertically   |
| Ctrl + w q | Close the current window      |

## Fold

| Shortcut | Explanation                              |
| -------- | ---------------------------------------- |
| zd       | Delete fold under th cursor              |
| zf       | Manualy define a fold up to motion       |
| za       | Toggle fold under the cursor             |
| zo       | Open fold under the cursor               |
| zc       | Close fold under the cursor              |
| zr       | Reduce (open) all folds by one level     |
| zm       | Fold more (close) all folds by one level |
| zi       | Toggle folding functionality             |

## NvimTree

| Shortcut | Explanation              |
| -------- | ------------------------ |
| g?       | Help                     |
| Ctrl + ] | Make current dir as root |

# NOT NESSECCARY

## Macros and Registers

| Shortcut | Explanation                                             |
| -------- | ------------------------------------------------------- |
| qa       | Start recording a macro in register 'a'                 |
| q        | Stop recording the macro                                |
| @a       | Execute the macro stored in register 'a'                |
| "ayw     | Yank (copy) the word under the cursor into register 'a' |
| "ap      | Paste the content of register 'a'                       |

## Buffers and Windows

| Shortcut      | Explanation               |
| ------------- | ------------------------- |
| :bnext or :bn | Go to the next buffer     |
| :bprev or :bp | Go to the previous buffer |
| :bd           | Delete the current buffer |
