## Traverse directory

``` python
for dirpath, dirs, files in os.walk(<target_path>):
    for f in files:
        print(os.path.join(dirpath, f))
```
