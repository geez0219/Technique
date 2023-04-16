## Arrow key remap

### Linux
* ref: https://superuser.com/questions/213051/remap-arrow-keys-to-winijkl-on-linux
* ref: https://www.youtube.com/watch?v=g_WUusDluLw


1. Create a remap file ~/.xmodmap

```
keycode 64 = Mode_switch
keysym j = j J Left
keysym l = l L Right
keysym i = i I Up
keysym k = k K Down
```

2. Run following command

```bash
xmodmap ~/.xmodmap
```
3. Go to ubuntu and search `Starup Application` and set `/usr/bin/xmodmap <path_to_.xmodmap>`


### Window
* https://blog.poychang.net/use-auto-hot-key-in-specific-program/

- download Autohotkey (https://www.autohotkey.com/)
- prepare .ahk file (https://stackoverflow.com/questions/30576432/remap-arrow-keys-onto-jkli-whenever-holding-down-a-certain-modifier-key)
```
NoEnv  ; Recommended for performance and compatibility with future AutoHotkey releases.
; #Warn  ; Enable warnings to assist with detecting common errors.
SendMode Input  ; Recommended for new scripts due to its superior speed and reliability.
SetWorkingDir %A_ScriptDir%  ; Ensures a consistent starting directory.

; AHK Command       ; key   = Effect        (Description)

; ALT Keypress Implied for all below

!i::Send {UP}       ; i UP          (Cursor up line)
!k::Send {DOWN}     ; k DOWN            (Cursor down line)

!j::Send {LEFT}     ; j LEFT        (Cursor left one character)
!l::Send {RIGHT}    ; l RIGHT       (Cursor right one character)

!h::Send {HOME}     ; h     ALT + RIGHT (Cursor to beginning of line)
!;::Send {END}      ; ; ALT + LEFT  (Cursor to end of line)

!u::Send ^{HOME}    ; h     SHIFT + HOME    (Cursor to beginning of document)
!o::Send ^{END}     ; o SHIFT + END (Cursor to end of document)
```

- Run at startup in Windows 10:
    1. Compile the script to *.exe.
    2. Put the shortcut of that exe in startup folder "%appdata%\Microsoft\Windows\Start Menu\Programs\Startup"
    3. That's all. Do NOT set it to run as admin. Programs in Win10 don't run at startup which are marked as run as admin.