
# launch_tensorboard
## lauch tensorboard on remote 
reference: https://stackoverflow.com/questions/37987839/how-can-i-run-tensorboard-on-a-remote-server
on the remote machine
- launch tensorboard
```
tensorboard --logdir="<tensorboard_dir_path>" --port==<remote_port/ex:8876>
```

on the local machine
- forward the remote port to local port using ssh
```
ssh -N -f -L localhost:<local_port/ex:8888>:localhost:<remote_port/ex:8876> <remote mahchine ssh name>
```



