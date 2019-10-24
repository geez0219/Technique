## Note
1. the -h tag in the following paragraph means humman-readable. it will make the terminal spit the memory size with K, M, G unit. 

## check system disk usage
```
df -h
```

## check usual disk usage

```
sudo du <target_dir> -d <max_depth> -a -h
```
1. it means list all files and directory under <target_dir> with max depth equal to <max_depth>
2. -a(all): not only checks directory but also the file
3. -d(max_depth): maximum search depth

```
sudo du <target_dir> -d <max_depth> -a | sort -n -r | head -n <top_K_to_show>
```
1. list top <top_K_to_show> files or dirs in the order of disk size (from large to small)
