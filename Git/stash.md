## Stash
Stash command can save the change to the "stash" list, and make the commit tree clean. Users can apply the change to any branch or drop the change.  
please refer: https://git-scm.com/docs/git-stash

## save the change

simplest: save the change without any message
``` bash
git stash 
```

save the change with message or even specifying file path
``` bash 
git stash push -m <string_of_message> [file_path]
```

## apply the stash

apply the change and keep the stash in the list
``` bash
git stash apply <stash_index> 
```
if the not specify index, it will assume 0


apply the change but remove the stash in the list
``` bash
git stash pop <stash_index>
```
if the not specify index, it will assume 0




