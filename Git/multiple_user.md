## using different user in specific folder
### this feature only there for new git version > 2.17.1

in `~/.gitconfig`
```
[user]
  name = geez0219
  email = geez0219@yahoo.com.tw

[includeIf "gitdir:<theGitPath>"]
  path = <theOtherGitConfig>
```
Note: the <theGitPath> folder should closing with "/"


in `<theOtherGitConfig>`
```
[user]
  name = <newName>
  email = <newEmail>
```

Now if you are located under <theGitPath> directory, your git information will be the one specified in <theOtherGitConfig>  
