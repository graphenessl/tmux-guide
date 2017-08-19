# tmux-guide
tmux: How to use tmux and cheat-sheet for tmux

![tmux cheatsheet guide](https://raw.githubusercontent.com/graphenessl/tmux-guide/master/terminal.png "tmux cheatsheet guide")

# Description:
**tmux** is a terminal multiplexer which is able to preserve terminal sessions. It is also able to split your terminal window horizontally or vertically. It is very useful when you have a lot of customizations or processes running in a terminal session, however you need to logout. The sessions can be saved, and then restored.

# Configuration:
Make sure to create a configuration in your local folder (you can leave it blank for now, but later you can add your settings there):

`~.tmux.conf`

If your username is John, then your file should be located at somewhere like:

`/home/john/.tmux.conf`

# Starting tmux:
Start **tmux** by typing in your terminal:

`tmux`

**tmux** does not start automatically. It is also perhaps not a good idea to do it too (since it can bloat you with multiple sessions). Once it starts, you will notice a new green (by default) bar line in the bottom of your terminal.
The first number indicates how many windows you have. The second number states the actual number of the window, which is displayed. On the rightmost end of the bar line there is a sample data like the current program which is running (usually your terminal, or the process, which has been run by the terminal), together with location and datetime.

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
### Swapping between panes:
Once you have already split your window to few panes, you can move between them via the arrow buttons <kbd>←</kbd>, <kbd>↑</kbd>, <kbd>→</kbd> and <kbd>↓</kbd>

**Example**:
<kbd>Ctrl</kbd>+<kbd>b</kbd> and then <kbd>↑</kbd> will move you to the pane above the current one.

### Sessions:
    tmux new -s session-name
    tmux list-sessions
    tmux attach -t session-name
