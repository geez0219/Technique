## show all remote
```
git remote -v
```
## add remote
```
git remote add <remote_name> <remore_url>
```

## set remote url

```
git remote set-url <remote_name> <new_URL>
```

### can disable the upstream push by setting url 

```
git remote set-url <remote_name> --push DISABLED
```
the url address is now "DISABLED" which is definitely not a available url, thus the push function is disabled.
