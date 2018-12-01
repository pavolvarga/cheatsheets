
# Vim commands

### Modes

| Command                                   | Meaning                                                           |
| :-------------------------------:         | :---------------------------------------------------------------: |
|                                           |                                                                   |
| `ESC`                                     | Return to normal mode                                             |
| `i`                                       | Enter into **insert** mode                                        |
| `v`                                       | Enter into visual mode                                            |
| `SHIFT + v`                               | Enter into visual line mode                                       |
| `SHIFT + :`                               | Enter into command mode                                           |

### Moving around

| Command                                   | Meaning                                                           |
| :-------------------------------:         | :---------------------------------------------------------------: |
|                                           |                                                                   |
| `h`                                       | Move cursor left                                                  |
| `l`                                       | Move cursor right                                                 |
| `j`                                       | Move cursor down                                                  |
| `k`                                       | Move cursor up                                                    |
|                                           |                                                                   |
| `H`                                       | Move to the top of a  screen                                      |
| `M`                                       | Move to the middle of a  screen                                   |
| `L`                                       | Move to the bottom of a screen                                    |
|                                           |                                                                   |
| `0`                                       | Jump to the start of a line                                       |
| `$`                                       | Jump to the end of a line                                         |                
| `^`                                       | Jump to the first non-blank character of a line                   |
| `g _`                                     | Jump to the last non-blank character of a line                    |
|                                           |                                                                   |
| `w`                                       | Jump forwards to start of a word                                  |
| `W`                                       | Jump forwards to start of a word with punctuation                 |
| `e`                                       | Jump forwards to end of a word                                    |
| `E`                                       | Jump forwards to end of a word with punctuation                   |
|                                           |                                                                   |
| `b`                                       | Jump backwards to start of a word                                 |
| `B`                                       | Jump backwards to start of a word with punctuation                |
| `g e`                                     | Jump backwards to end of a word                                   |
| `g E`                                     | Jump backwards to end of a word with punctuation                  |
|                                           |                                                                   |
| `f x`                                     | Jump to the next occurence of character *x*                       |
| `t x`                                     | Jump to character before the next occurence of character *x*      |
| `F x`                                     | Jump to the previous occurence of character *x*                   |
| `T x`                                     | Jump to character after the previous occurence of character *x*   |
|                                           |                                                                   |
| `;`                                       | Repeat previous `f`, `t`, `F`, `T` movement                       |
| `,`                                       | Repeat previous `f`, `t`, `F`, `T` movement backwards             |
|                                           |                                                                   |
| `%`                                       | Jump to mathing opening or closing ( [ {                          |

### Editing

| Command                                   | Meaning                                                           |
| :---------------------------------------: | :---------------------------------------------------------------: |
|                                           |                                                                   |   
| `i`                                       | Insert before cursor                                              |
| `I`                                       | Insert at the beginning of a line                                 |
| `a`                                       | Append after cursor                                               |
| `A`                                       | Append at the end of a line                                       |
|                                           |                                                                   |
| `r`                                       | Replace character at cursor                                       |
| `x`                                       | Delete character at cursor                                        |
| `s`                                       | Substitute character at cursor                                    |
|                                           |                                                                   |   
| `O`                                       | Open newline above the current line                               |
| `o`                                       | Open newline below the current line                               |
|                                           |                                                                   |
| `d a w`                                   | Delete a word                                                     |
| `c a w`                                   | Change a word                                                     |
|                                           |                                                                   |
| `c w`                                     | Change to the end of a word                                       |
| `c b`                                     | Change to the begining of a word                                  |
|                                           |                                                                   |
| `d i ( [ { ' " <` or `d i ) ] } ' " >`    | Delete between () , [] , {} , '' , "" , <>                        |
| `c i ( [ { ' " <` or `c i ) ] } ' " >`    | Change between () , [] , {} , '' , "" , <>                        |
|                                           |                                                                   |
| `~`                                       | Switch case                                                       | 
|                                           |                                                                   |
| `c c` or `S`                              | Change entire line                                                |
| `c $`                                     | Change to the end of a line                                       |
| `c 0`                                     | Change to the beginging of a line                                 |

### Searching

| Command                                   | Meaning                                                           |
| :---------------------------------------: | :---------------------------------------------------------------: |
|                                           |                                                                   |
| `/`                                       | Opend the search prompt                                           |
| `n`                                       | Next search match                                                 |
| `N`                                       | Previous search match                                             |

### Macros

| Command                                   | Meaning                                                           |
| :---------------------------------------: | :---------------------------------------------------------------: |
|                                           |                                                                   |
| `q a`                                     | Start recording macro *a*                                         |
| `q`                                       | Stop recording macro *a*                                          |
| `@`                                       | Run macro *a*                                                     |
| `@@`                                      | Re-run the last run macro                                         |

### Undo & Redo

| Command                                   | Meaning                                                           |
| :---------------------------------------: | :---------------------------------------------------------------: |
|                                           |                                                                   |
| `u`                                       | Undo                                                              |
| `CTRL + u`                                | Redo                                                              |
