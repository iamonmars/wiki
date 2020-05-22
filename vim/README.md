# Vim Editor

[Example of vimrc file](./vimrc)

## Install Plugins


## Save and quit
```
:w  # to write
:q  # to quit
```

## Moving around
```
h   # to left
j   # to down
k   # to up
l   # to right

w   # moving forward by word
e   # moving forward to the end of the word
b   # moving backwards to the beginning of the word

{   # move back by one paragraph
}   # move forward by one paragraph

gg  # move to the top of the file
G   # move to the bottom of the file

_   # move to the beginning of the line
$   # move to the end of the line
```

## Editing
```
cw  # change next word
dw  # delete next word

cc  # create a new line
dd  # delete an entire line

a               # places you in insert mode after the cursor
s               # s deletes a single character
d + a movement  # delete through the move
```

## Organize the workspace

### Buffers
```
:ls # list existing buffers
:bd # delete specific buffer
```

### Windows
```
:sp # split horizontally a new window
:vs # split vertically a new window
```

**Moving in diferent windows**
```
Ctrl + h    # Left window
Ctrl + j    # Down window
Ctrl + k    # Up window
Ctrl + l    # Right window
```

### Folds
```
zo  # open folded lines
zc  # close folded lines
```

## Navigate
```
:e .        # explore directory
:NERDTree   # list files in the directory
Ctrl + p    # open CtrlP file search input
```

## Search

**In a file**
```
/           # search for a match by typing in
n           # go to the next match
N           # go to the previous match
:noh        # clear searched highlights
\ + \ + w   # by easy motion
```

**Across files**

Firstly, we have to install ack
```$ sudo apt-get install ack-grep```

```:Ack --extension word   # :Ack --python Animal```

## Copy and paste
```
y + a movement  # copy
yy              # copy contents of current line
p               # paste
```
