### launch new tmux session
    tmux new -s myname = start session myname

### Keysettings
    <prefix> Key = space
    <Leader> Key = capslock+a


# Scrollmode
    <Leader> [ = Scrollmode aktivieren + vim keybindings steuern
    v = markierung im Scrollmodus starten
    y = markierung im Scrollmodus ins clipboard kopieren


# Windows (tabs)
    c = create window
    w = list windows
    n =  next window
    p =  previous window
    f =  find window
    , =  name window
    & =  kill window

# Panes (Splits)
    %  = vertical split
    "  = horizontal split
    o  = swap panes
    q  = show pane numbers
    x  = kill pane
    +  = break pane into window (e.g. to select text by mouse to copy)
    -  = restore pane from window
    ⍽  = space - toggle between layouts
    <prefix> q = (Show pane numbers, when the numbers show up type the key to goto that pane)
    <prefix> { = (Move the current pane left)
    <prefix> } = (Move the current pane right)
    <prefix> z = toggle pane zoom
