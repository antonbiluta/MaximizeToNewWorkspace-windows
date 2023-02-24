# Maximize to the new Workspace like MacOS

## Overview
This script implements the function of expanding the window in a new workspace, as it works on Mac OS

## Annotation
When the window is maximized 
1. A new desktop is created with the process name of the maximized window
2. The current window is transferred to the new desktop
3. You are automatically transferred to a new desktop

When you restore the window
1. The name of the current window and the name of the desktop are checked
    - If the names match:
        1. The window returns to the main (first) working screen
        2. You are automatically returned to the main (first) screen
        3. The desktop is being deleted
    - If the names don't match - nothing

*In the future, it is planned to make a check in case the window is closed or minimized*

## Running
[Install AutoHotkey](https://autohotkey.com/download/) v2 and run `maximizeScript.ahk`


## Running on boot
1. Press <kbd>Win</kbd> + <kbd>R</kbd>, enter `shell:startup`, then click <kbd>OK</kbd>
2. Create a shortcut to the `maximizeScript.ahk` file here

## Credits
- Thanks to [Ciantic/VirtualDesktopAccessor](https://github.com/Ciantic/VirtualDesktopAccessor) (DLL)