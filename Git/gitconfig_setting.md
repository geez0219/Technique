``` .gitconfig
[user]
      name = Yun-Chan Tsai
      email = Yun-Chan.Tsai@ge.com

# setting up the new user information for specific folder
[includeIf "gitdir:/mnt/c/model_converter_project/"]
      path = ~/work/.gitconfig

[credential]
      helper = cache --timeout=28800
  
```
