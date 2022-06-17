# Modes

`Esc` Normal: for navigation/commands

`i` Insert: editing

`v` Visual: copying

# Navigation

Add a number before any command to multiply it

`h` Left

`j` Down

`k` Up

`l` Right

`w` Go to start of next token

`e` Go to end of next token

`b` Go to start of previous token

`0` Go to start of line

`$` Go to end of line

`20G` Go to start of line 20

`gg` Go to top line of file

`G` Go to bottom line of file

`zz` Vertically centre current cursor

`f` Move to a particular letter in a line, e.g. `ft`

# Actions

`p` Put after

`P` Put before

`u` Undo

`U` Undo all changes on current line

`Ctrl-R` Redo

`y` Yank (Copy) e.g. `y2j` is yank everything from this line down to the one on line 2 below (i.e. actually 3 lines)

`yw` Yank one word

`yy` Yank whole line e.g. `2yy` is yank two lines

`y}` Yank to end of this closure

### Changing text

`ce` Change from cursor to end of word

`c$` Change from cursor to end of line

`R` Replace all characters with following letters

`r` Replace single character with following letter, e.g. `re`

### Deleting text (will also yank)

`x` Delete character you're on

`d` Delete mode

`dw` Delete to start of next word

`de` Delete from cursor to end of word

`D` Delete to end of the line

`dd` Delete whole line, e.g. `2dd` will delete current line and one below

`cc` Delete whole line and go into `insert` mode

### Searching text

`/` Search in forward direction

`?` Search in backward direction

`n` Go to next search result

`N` Go to previous search result

### Substituting text

`:s/wrong/right` Substitute the first instance of 'wrong' on a line with 'right'

`:s/wrong/right/g` Substitute every instance of 'wrong' on a line with 'right'

`:2,5s/wrong/right/g` Substitute every instance of 'wrong' between lines 2 and 5 with 'right'

`:%s/wrong/right/g` Substitute every instance of 'wrong' in a file with 'right'

`:%s/wrong/right/gc` Prompt to individually substitute every instance of 'wrong' in a file with 'right'

# Shortcuts

`o` Make new line underneath and enter Insert mode

`O` Make new line above and enter Insert mode

`I` Insert at start of line

`a` Append after cursor

`A` Append at end of line

`%` When on a `(, [ or {` finds the matching bracket
