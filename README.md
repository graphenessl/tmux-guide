# tmux-guide
tmux: How to use tmux and cheat-sheet for tmux

# Description:
**tmux** is a terminal multiplexer which is able to preserve terminal sessions. It is also able to split your terminal window horizontally or programatically.

# Configuration:
Make sure to create a configuration in your local folder:

`~.tmux.conf`

If your username is John, then your file should be located at somewhere like:

`/home/john/.tmux.conf`

# Cheat sheet:
### Launching a command:
    Ctrl+b <command>
    
NOTE: First press together keyboard keys <kbd>Ctrl</kbd> and <kbd>b</kbd> buttons. Then release your fingers from then and press <kbd>b</kbd>. Do not laugh, a lot of people don't get it right. ;) 

# Commands
### Windows:
    c	- window: create
    ,	- window: rename
    p	- window: previous
    n	- window: next
    w	- window: select available windows
    s	- window: list all sessions

### Splits:
    %	- Split: Vertical
    "	- Split: Horizontal
    
#### Misc
    :	- Commands: Run a custom named command which you have created (e.g. "split-windows")

### Panes:
    q  - Pane: Show numbers
    x  - Pane: Kill
    o  - Panes: Swap

### Sessions:
    tmux new -s session-name
    tmux list-sessions
    tmux attach -t session-name
