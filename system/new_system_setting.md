## Arrow key remap

### Linux
* ref: https://superuser.com/questions/213051/remap-arrow-keys-to-winijkl-on-linux
* ref: https://www.youtube.com/watch?v=g_WUusDluLw


1. create a remap file ~/.xmodmap

```
keycode 64 = Mode_switch
keysym j = j J Left
keysym l = l L Right
keysym i = i I Up
keysym k = k K Down
```

2. >>> xmodmap ~/.xmodmap

3. Go to ubuntu and search `Starup Application` and set `/usr/bin/xmodmap <path_to_.xmodmap>`
