# TMUX

# L = <Leader> = Ctrl + f

## Sessions

| Shortcut                                   | Explanation                                 |
| ------------------------------------------ | ------------------------------------------- |
| tmux                                       | Start a new session                         |
| tmux new -s mysession or :new -s mysession | Start a new session with the name mysession |
| tmux kill-session -t mysession             | Kill/delete session mysession               |
| tmux fill-session -a                       | Kill/delete all sessions but the current    |
| tmux fill-session -a -t mysession          | Kill/delete all sessions but mysession      |
| L $                                        | Rename session                              |
| L d                                        | Detach from session                         |
| tmux ls / L s                              | Show all sessions                           |
| tmux a                                     | Attach to last session                      |
| tmux a -t mysession                        | Attach to a session with th name mysession  |
| L (                                        | Move to previous session                    |
| L )                                        | Move to next session                        |

## Windows

| Shortcut                          | Explanation                                                     |
| --------------------------------- | --------------------------------------------------------------- |
| tmux new -s mysession -n mywindow | Start a new session with the name mysession and window mywindow |
| l c                               | Create window                                                   |
| l ,                               | Rename current window                                           |
| l &                               | Close current window                                            |
| l p                               | Previous window                                                 |
| l n                               | Next window                                                     |
| l 0 ... 9                         | Switch/select window my number                                  |
| swap-window -s 2 -t 1             | Reorder window, swap window number 2(src) and 1(dst)            |
| swap-window -t -1                 | Move current window to the left by one position                 |

## Panes

| Shortcut                         | Explanation                                          |
| -------------------------------- | ---------------------------------------------------- |
| L ;                              | Toggle last active Panes                             |
| L % / L V                        | Split pane vertically                                |
| L " / L S                        | Split pane horizontally                              |
| L {                              | Move the current pane left                           |
| L }                              | Move the current pane right                          |
| L <Left> (<Right>, <Up>, <Down>) | Switch to pane to the direction                      |
| setw synchronize-panes           | Toggle synchronize-panes (send command to all panes) |
| L Spacebar                       | Toggle between pane layouts                          |
| L o                              | Switch to next pane                                  |
| L q                              | Show pane numbers                                    |
| L q 0 ... 9                      | Switch/select pane by number                         |
| L z                              | Toggle pane zoom                                     |
| L !                              | Convert pane into a window                           |
| L <Up> (<Down>)                  | Resize current pane height (hold three keys)         |
| L <Right> (<Left>)               | Resize current pane width (hold three keys)          |
| L x                              | Close current pane                                   |

## Copy Mode

| Shortcut             | Explanation                                      |
| -------------------- | ------------------------------------------------ |
| setw -g mode-keys vi | Use vi keys in buffer                            |
| L [                  | Enter copy mode                                  |
| L PgUp               | Enter copy mode and scroll one page up           |
| q                    | Quit mode                                        |
| Spacebar             | Start selection                                  |
| Esc                  | Clear selection                                  |
| Enter                | Copy selection                                   |
| L ]                  | Paste contents of buffer_0                       |
| show-buffer          | Display buffer_0 contents                        |
| capture-pane         | Copy entire visible contents of pane to a buffer |
| list-buffers         | Show all buffers                                 |
| choose-buffer        | Show all buffers and paste selected              |
| save-buffer buf.txt  | Save buffer contents to buf.txt                  |
| delete-buffer -b 1   | Delete buffer_1                                  |

## Misc

| Shortcut       | Explanation                              |
| -------------- | ---------------------------------------- |
| L :            | Entere command mode                      |
| set -g OPTION  | Set OPTION for all sessions              |
| setw -g OPTION | Set OPTION for all windows               |
| tmux info      | Show every session, window, pane, etc... |
| L ?            | Show shortcuts                           |

## General

| Shortcut                          | Explanation                                                |
| --------------------------------- | ---------------------------------------------------------- |
| C-f C-o                           | Rotate through the panes                                   |
| C-f C-z                           | Suspend the current client                                 |
| C-f Space                         | Select next layout                                         |
| C-f !                             | Break pane to a new window                                 |
| C-f "                             | Split window vertically                                    |
| C-f #                             | List all paste buffers                                     |
| C-f $                             | Rename current session                                     |
| C-f %                             | Split window horizontally                                  |
| C-f &                             | Kill current window                                        |
| C-f '                             | Prompt for window index to select                          |
| C-f (                             | Switch to previous client                                  |
| C-f )                             | Switch to next client                                      |
| C-f ,                             | Rename current window                                      |
| C-f -                             | Delete the most recent paste buffer                        |
| C-f .                             | Move the current window                                    |
| C-f /                             | Describe key binding                                       |
| C-f 0                             | Select window 0                                            |
| C-f 1                             | Select window 1                                            |
| C-f 2                             | Select window 2                                            |
| C-f 3                             | Select window 3                                            |
| C-f 4                             | Select window 4                                            |
| C-f 5                             | Select window 5                                            |
| C-f 6                             | Select window 6                                            |
| C-f 7                             | Select window 7                                            |
| C-f 8                             | Select window 8                                            |
| C-f 9                             | Select window 9                                            |
| C-f :                             | Prompt for a command                                       |
| C-f ;                             | Move to the previously active pane                         |
| C-f =                             | Choose a paste buffer from a list                          |
| C-f ?                             | List key bindings                                          |
| C-f C                             | Customize options                                          |
| C-f D                             | Choose and detach a client from a list                     |
| C-f E                             | Spread panes out evenly                                    |
| C-f M                             | Clear the marked pane                                      |
| C-f [                             | Enter copy mode                                            |
| C-f ]                             | Paste the most recent paste buffer                         |
| C-f c                             | Create a new window                                        |
| C-f d                             | Detach the current client                                  |
| C-f f                             | Search for a pane                                          |
| C-f i                             | Display window information                                 |
| C-f m                             | Toggle the marked pane                                     |
| C-f n                             | Select the next window                                     |
| C-f o                             | Select the next pane                                       |
| C-f p                             | Select the previous window                                 |
| C-f q                             | Display pane numbers                                       |
| C-f s                             | Choose a session from a list                               |
| C-f w                             | Choose a window from a list                                |
| C-f x                             | Kill the active pane                                       |
| C-f z                             | Zoom the active pane                                       |
| C-f {                             | Swap the active pane with the pane above                   |
| C-f }                             | Swap the active pane with the pane below                   |
| C-f ~                             | Show messages                                              |
| C-f DC                            | Reset so the visible part of the window follows the cursor |
| C-f PPage                         | Enter copy mode and scroll up                              |
| C-f Up                            | Select the pane above the active pane                      |
| C-f Down                          | Select the pane below the active pane                      |
| C-f Left                          | Select the pane to the left of the active pane             |
| C-f Right                         | Select the pane to the right of the active pane            |
| C-f M-1                           | Set the even-horizontal layout                             |
| C-f M-2                           | Set the even-vertical layout                               |
| C-f M-3                           | Set the main-horizontal layout                             |
| C-f M-4                           | Set the main-vertical layout                               |
| C-f M-5                           | Select the tiled layout                                    |
| C-f M-n                           | Select the next window with an alert                       |
| C-f M-o                           | Rotate through the panes in reverse                        |
| C-f M-p                           | Select the previous window with an alert                   |
| C-f M-Up                          | Resize the pane up by 5                                    |
| C-f M-Down                        | Resize the pane down by 5                                  |
| C-f M-Left                        | Resize the pane left by 5                                  |
| C-f M-Right                       | Resize the pane right by 5                                 |
| C-f C-Up                          | Resize the pane up                                         |
| C-f C-Down                        | Resize the pane down                                       |
| C-f C-Left                        | Resize the pane left                                       |
| C-f C-Right                       | Resize the pane right                                      |
| C-f S-Up, S-Down, S-Left, S-Right | Move the visible part of the window up, down, left, right  |
