## Agent forward
This is useful when you have access of two machine and need to send files from one to the another(say A to B). </br>
You don't want to save B key to A machine. [ref: https://dev.to/levivm/how-to-use-ssh-and-ssh-agent-forwarding-more-secure-ssh-2c32]

1. create an ssh agent
```
eval "$(ssh-agent -s)"
```
2. add the key to that machine

```
ssh-add <path_to_key(~/.ssh/gehc-explorer.pem)> 
```

3. link to A machine using ssh 
```
ssh -A <user>@<ip>
```
or 
```
ssh <user>@<ip>
```

if you already set up the .ssh config file as 

``` config
Host A
  ...
  ForwardAgent yes
  ...

```

