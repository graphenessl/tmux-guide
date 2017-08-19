# tmux-guide
tmux: How to use tmux and cheat-sheet for tmux

Cheat sheet:
============

Ctrl+b <command>

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
q  show pane numbers
x  kill pane
o  swap panes

Sessions:
tmux new -s session-name
tmux list-sessions
tmux attach -t session-name
