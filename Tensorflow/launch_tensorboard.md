
# launch_tensorboard
## lauch tensorboard on remote 

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



