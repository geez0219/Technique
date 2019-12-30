## prefix
the tmux has a hot key that recurrently being used. It is default Ctrl + B.
In the following session prefix == Ctrl + B


## session

### get into tmux session
```
tmux 
```
### create a tmux session with specific name
```
tmux new -s <session_name>
```

### leave tmux session (but the session is still running) 
```
prefix + D
```

### attach back to tmux session
```
tmux attach -t <session_name>
```

### show all tmux session 
```
tmux ls
```

### exit the tmux session (the session will be ended)
```
exit
```

## window
### create a new window in same session
```
prefix + c 
```

### switch to different window
```
prefix + <window_index>
```

### rename the window
```
prefix + ,
```

### exit the window
```
exit
```

## split 
### split the terminal horizontally
```
prefix + %
```

### split the terminal vertically
```
prefix + "
```
