# tmux-guide
tmux: How to use tmux and cheat-sheet for tmux

Configuration:
============
Make sure to create a configuration in your local folder:
    ~.tmux.conf

If your username is John, then your file should be located at somewhere like:
    /home/john/.tmux.conf

Cheat sheet:
============
    Ctrl+b <command>
NOTE: First press together [Ctrl] and [b] buttons. Then release your fingers from then and press [b].

Commands
============
    Windows:
    c	- window: create
    ,	- window: rename
    p	- window: previous
    n	- window: next
    w	- window: select available windows
    s	- window: list all sessions

Splits:
    %	- Split: Vertical
    "	- Split: Horizontal

Misc:
    :	- Commands: Run a custom named command which you have created (e.g. "split-windows")

Panes:
    q  - Pane: Show numbers
    x  - Pane: Kill
    o  - Panes: Swap

Sessions:
    tmux new -s session-name
    tmux list-sessions
    tmux attach -t session-name
