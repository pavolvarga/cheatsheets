# Vim commands

## Modes

| Command                                           | Meaning                                                               |
| :-----------------------------------------------: | :-------------------------------------------------------------------: |
|                                                   |                                                                       |
| `ESC`                                             | Return to **normal** / **command** mode                               |
| `i`                                               | Enter into **insert** mode                                            |
| `v`                                               | Enter into visual mode                                                |
| `SHIFT + v`                                       | Enter into visual line mode                                           |
| `CTRL + v`                                        | Einter into visual block mode                                         |
| `SHIFT + :`                                       | Enter into command mode                                               |
| `:`                                               | Enter into command line mode                                          |

## Moving around

| Command                                           | Meaning                                                               |
| :-----------------------------------------------: | :-------------------------------------------------------------------: |
|                                                   |                                                                       |
| `h`                                               | Move cursor left                                                      |
| `l`                                               | Move cursor right                                                     |
| `j`                                               | Move cursor down                                                      |
| `k`                                               | Move cursor up                                                        |
|                                                   |                                                                       |
| `CTRL + F`                                        | Move page down                                                        |
| `CTRL + B`                                        | Move page up                                                          |
|                                                   |                                                                       |
| `H`                                               | Move to the top of a  screen                                          |
| `M`                                               | Move to the middle of a  screen                                       |
| `L`                                               | Move to the bottom of a screen                                        |
|                                                   |                                                                       |
| `0`                                               | Jump to the start of a line                                           |
| `$`                                               | Jump to the end of a line                                             |
| `^`                                               | Jump to the first non-blank character of a line                       |
| `g _`                                             | Jump to the last non-blank character of a line                        |
|                                                   |                                                                       |
| `g g`                                             | Jump to the first line                                                |
| `G`                                               | Jump to the last line                                                 |
| `g g 10` or `G 10`                                | Jump to the *10th* line                                               |
|                                                   |                                                                       |
| `w`                                               | Jump forwards to start of a word                                      |
| `W`                                               | Jump forwards to start of a word with punctuation                     |
| `e`                                               | Jump forwards to end of a word                                        |
| `E`                                               | Jump forwards to end of a word with punctuation                       |
|                                                   |                                                                       |
| `b`                                               | Jump backwards to start of a word                                     |
| `B`                                               | Jump backwards to start of a word with punctuation                    |
| `g e`                                             | Jump backwards to end of a word                                       |
| `g E`                                             | Jump backwards to end of a word with punctuation                      |
|                                                   |                                                                       |
| `f x`                                             | Jump to the next occurence of character *x*                           |
| `t x`                                             | Jump to character before the next occurence of character *x*          |
| `F x`                                             | Jump to the previous occurence of character *x*                       |
| `T x`                                             | Jump to character after the previous occurence of character *x*       |
|                                                   |                                                                       |
| `;`                                               | Repeat previous `f`, `t`, `F`, `T` movement                           |
| `,`                                               | Repeat previous `f`, `t`, `F`, `T` movement backwards                 |
|                                                   |                                                                       |
| `%`                                               | Jump to mathing opening or closing ( [ {                              |
|                                                   |                                                                       |
| `z t`                                             | Put current line to the top of screen                                 |
| `z z`                                             | Put current line to the middle of screen                              |
| `z b`                                             | Put current line to the bottom of screen                              |

## Editing

| Command                                           | Meaning                                                               |
| :-----------------------------------------------: | :-------------------------------------------------------------------: |
|                                                   |                                                                       |
| `i`                                               | Insert before cursor                                                  |
| `I`                                               | Insert at the beginning (first non blank character) of a line         |
| `a`                                               | Append after cursor                                                   |
| `A`                                               | Append at the end of a line                                           |
|                                                   |                                                                       |
| `r`                                               | Replace character at cursor                                           |
| `R`                                               | Start replacing (as writing new text over existing one)               |
| `x`                                               | Delete character at cursor                                            |
| `X`                                               | Delete character before cursor                                        |
| `s`                                               | Substitute character at cursor                                        |
|                                                   |                                                                       |
| `O`                                               | Open newline above the current line                                   |
| `o`                                               | Open newline below the current line                                   |
|                                                   |                                                                       |
| `d w`                                             | Delete to the end of a word                                           |
| `d b`                                             | Delete to the begining of a word                                      |
| `c w`                                             | Change to the end of a word                                           |
| `c b`                                             | Change to the begining of a word                                      |
|                                                   |                                                                       |
| `d a w`                                           | Delete a word (including boundary / space)                            |
| `c a w`                                           | Change a word (including boundary / space)                            |
| `d i w`                                           | Delete inner word (excluding boundary / space)                        |
| `c i w`                                           | Change inner word (excluding boundary / space)                        |
|                                                   |                                                                       |
| `d a s`                                           | Delete a sentence (including boundary)                                |
| `c a s`                                           | Change a sentence (including boundary)                                |
| `d i s`                                           | Delete a sentence (excluding boundary)                                |
| `c i s`                                           | Change a sentence (excluding boundary)                                |
|                                                   |                                                                       |
| `d a p`                                           | Delete a paragprah (including boundary / blank line)                  |
| `c a p`                                           | Change a paragprah (including boundary / blank line)                  |
| `d i p`                                           | Delete a paragprah (excluding boundary / blank line)                  |
| `c i p`                                           | Change a paragprah (excluding boundary / blank line)                  |
|                                                   |                                                                       |
| `d a t`                                           | Delete a tag (including boundary)                                     |
| `c a t`                                           | Change a tag (including boundary)                                     |
| `d i t`                                           | Delete a tag (excluding boundary)                                     |
| `c i t`                                           | Change a tag (excluding boundary)                                     |
|                                                   |                                                                       |
| `d a B`                                           | Delete a block (including boundary)                                   |
| `c a B`                                           | Change a block (including boundary)                                   |
| `d i B`                                           | Delete a block (excluding boundary)                                   |
| `c i B`                                           | Change a block (excluding boundary)                                   |
|                                                   |                                                                       |
| `d a ( [ { < ' " `` ` or `d a ) ] } > ' " `` `    | Delete between () , [] , {} , <> '' , "" , `` (including boundaries)  |
| `c a ( [ { < ' " `` ` or `c a ) ] } > ' " `` `    | Change between () , [] , {} , <> '' , "" , `` (including boundaries)  |
| `d i ( [ { < ' " `` ` or `d i ) ] } > ' " `` `    | Delete between () , [] , {} , <> '' , "" , `` (excluding boundaries)  |
| `c i ( [ { < ' " `` ` or `c i ) ] } > ' " `` `    | Change between () , [] , {} , <> '' , "" , `` (excluding boundaries)  |
|                                                   |                                                                       |
| `~`                                               | Switch case                                                           |
| `g ~ w`                                           | Switch case for entire word                                           |
| `g ~ ~`                                           | Switch case for entire line                                           |
|                                                   |                                                                       |
| `g U w`                                           | Turn all characters in word uppercase                                 |
| `g U U`                                           | Turn all characters in line uppercase                                 |
| `g u w`                                           | Turn all characters in word lowercase                                 |
| `g u u`                                           | Turn all characters in line lowercase                                 |
|                                                   |                                                                       |
| `c c` or `S`                                      | Change entire line                                                    |
| `c $` or `C`                                      | Change to the end of a line                                           |
| `c 0`                                             | Change to the beginnging of a line                                    |
|                                                   |                                                                       |
| `d d`                                             | Delete / cut entire line                                              |
| `d $` or `D`                                      | Delete / cut to the end of a line                                     |
| `d 0`                                             | Delete / cut to the beginning of a line                               |
|                                                   |                                                                       |
| `y y`                                             | Copy / yank entire line                                               |
| `y $`                                             | Copy / yank to the end of a line                                      |
| `y 0`                                             | Copy / yank to the beginning of a line                                |
|                                                   |                                                                       |
| `J`                                               | Join lines (with spaces)                                              |
| `g J`                                             | Join lines (without spaces)                                           |
|                                                   |                                                                       |
| `> >`                                             | Intend to the right                                                   |
| `< <`                                             | Intend to the left                                                    |

## Searching

| Command                                           | Meaning                                                               |
| :-----------------------------------------------: | :-------------------------------------------------------------------: |
|                                                   |                                                                       |
| `/{pattern}`                                      | Search *pattern* forwards                                             |
| `?{pattern}`                                      | Search *pattern* backwards                                            |
| `*`                                               | Forward search for word (under cursor)                                |
| `#`                                               | Backward search for word (under cursor)                               |
| `n`                                               | Next search match                                                     |
| `N`                                               | Previous search match                                                 |

## Macros

| Command                                           | Meaning                                                               |
| :-----------------------------------------------: | :-------------------------------------------------------------------: |
|                                                   |                                                                       |
| `q a`                                             | Start recording macro into register *a*                               |
| `q`                                               | Stop recording macro to register *a*                                  |
| `@ A`                                             | Append to macro in register *a*                                       |
| `@ a`                                             | Run macro in register *a*                                             |
| `@@`                                              | Re-run the last run macro                                             |

## Undo & Redo & Repeating

| Command                                           | Meaning                                                               |
| :-----------------------------------------------: | :-------------------------------------------------------------------: |
|                                                   |                                                                       |
| `u`                                               | Undo                                                                  |
| `CTRL + u`                                        | Redo                                                                  |
| `.`                                               | Repeat the previous command (like 'delete a word')                    |

## Copy & Cut & Paste / Yank & Delete & Put

| Command                                           | Meaning                                                               |
| :-----------------------------------------------: | :-------------------------------------------------------------------: |
|                                                   |                                                                       |
| `p`                                               | Put text after / below cursor                                         |
| `P`                                               | Put text before / above cursor                                        |
|                                                   |                                                                       |
| `" j y y`                                         | Copy line into register *j*                                           |
| `" 4 y y`                                         | Copy line into register *4*                                           |
|                                                   |                                                                       |
| `" j p`                                           | Put content of register *j* after cursor                              |
| `" 4 p`                                           | Put content of register *4* after cursor                              |

## Visual mode

| Command                                           | Meaning                                                               |
| :-----------------------------------------------: | :-------------------------------------------------------------------: |
|                                                   |                                                                       |
| `v`                                               | Start visual mode                                                     |
| `o`                                               | Jump to the end of sected text                                        |
| `O`                                               | Jump to the beginning of sected text                                  |
| `g v`                                             | Reselect previously selected text                                     |

## Command line mode

| Command                                           | Meaning                                                               |
| :-----------------------------------------------: | :-------------------------------------------------------------------: |
|                                                   |                                                                       |
| `: q`                                             | Quit vim                                                              |
| `: q!`                                            | Quit vim without saving changes                                       |
|                                                   |                                                                       |
| `: w`                                             | Save changes                                                          |
| `: wq`                                            | Save changes and quit                                                 |
|                                                   |                                                                       |
| `: 44<Enter>`                                     | Jump to the line *44*                                                 |
| `: $<Enter>`                                      | Jump to the last line                                                 |
| `: 0<Enter>`                                      | Jump to the first line                                                |
|                                                   |                                                                       |
| `: help [text]`                                   | Open help                                                             |
| `: reg [register(s)]`                             | Show content of registers                                             |
|                                                   |                                                                       |
| `: [range]s/old/new/[flags]`                      | Substitue *old* text with *new* text                                  |
| `: %s/old/new/g`                                  | Substitue *old* text with *new* text in entire file                   |
