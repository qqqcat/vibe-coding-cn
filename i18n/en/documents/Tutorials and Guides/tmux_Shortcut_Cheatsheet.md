## tmux Shortcut Cheatsheet (Prefix Ctrl+b)

### Sessions
| Operation | Shortcut |
|-----------|----------|
| Detach Session | d |
| List Sessions | s |
| Rename Session | $ |

### Windows
| Operation | Shortcut |
|-----------|----------|
| New Window | c |
| Close Window | & |
| Next Window | n |
| Previous Window | p |
| Switch to Window N | 0-9 |
| Rename Window | , |
| List Windows | w |

### Panes
| Operation | Shortcut |
|-----------|----------|
| Split Pane Horizontal | % |
| Split Pane Vertical | " |
| Switch Pane | Arrow keys |
| Close Pane | x |
| Display Pane Numbers | q |
| Toggle Pane Fullscreen/Restore | z |
| Resize | Ctrl+Arrow keys |
| Swap Panes | { / } |
| Break Pane to New Window | ! |

### Others
| Operation | Shortcut |
|-----------|----------|
| Enter Copy Mode | [ |
| Paste | ] |
| Show Time | t |
| Command Mode | : |
| List Shortcuts | ? |

### Command Line
bash
tmux                  # New session
tmux new -s name      # New named session
tmux ls               # List sessions
tmux attach -t name   # Attach session
tmux kill-session -t name  # Kill session