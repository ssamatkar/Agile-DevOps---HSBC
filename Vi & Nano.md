
### **`vi` (or `vim`) Cheatsheet**

#### **Modes:**
- **Normal Mode**: For navigation and commands (default mode).
- **Insert Mode**: For text entry (press `i` to enter).
- **Visual Mode**: For text selection (press `v` to enter).

#### **Common Commands:**

- **Entering Insert Mode**:
  - `i` : Insert before cursor
  - `I` : Insert at the beginning of the line
  - `a` : Append after cursor
  - `A` : Append at the end of the line
  - `o` : Open a new line below the current line
  - `O` : Open a new line above the current line

- **Exiting Insert Mode**:
  - `ESC` : Return to Normal Mode

- **Saving and Exiting**:
  - `:w` : Save file
  - `:q` : Quit
  - `:wq` or `:x` : Save and quit
  - `:q!` : Quit without saving

- **Navigation**:
  - `h` : Move left
  - `j` : Move down
  - `k` : Move up
  - `l` : Move right
  - `0` : Move to the beginning of the line
  - `$` : Move to the end of the line
  - `G` : Move to the end of the file
  - `gg` : Move to the beginning of the file

- **Editing**:
  - `x` : Delete character under the cursor
  - `dd` : Delete the current line
  - `yy` : Copy (yank) the current line
  - `p` : Paste after the cursor
  - `u` : Undo
  - `Ctrl+r` : Redo

- **Searching**:
  - `/text` : Search for `text`
  - `n` : Next search result
  - `N` : Previous search result

- **Replacing**:
  - `r<char>` : Replace the character under the cursor with `<char>`
  - `R` : Enter Replace mode

### **`nano` Cheatsheet**

#### **Basic Commands:**
- **Starting Nano**:
  - `nano filename` : Open or create a file with the given name

- **Saving and Exiting**:
  - `Ctrl+O` : Save file (press Enter to confirm)
  - `Ctrl+X` : Exit Nano (prompt to save if there are unsaved changes)

- **Navigation**:
  - `Ctrl+A` : Move to the beginning of the line
  - `Ctrl+E` : Move to the end of the line
  - `Ctrl+Y` : Move up one page
  - `Ctrl+V` : Move down one page

- **Editing**:
  - `Ctrl+K` : Cut the current line
  - `Ctrl+U` : Paste the cut line
  - `Ctrl+J` : Justify the current paragraph
  - `Ctrl+C` : Display the current cursor position

- **Searching**:
  - `Ctrl+W` : Search for text
  - `Ctrl+T` : Replace text (after searching)

- **Other Useful Commands**:
  - `Ctrl+G` : Display the help screen
  - `Ctrl+_` : Go to a specific line number

