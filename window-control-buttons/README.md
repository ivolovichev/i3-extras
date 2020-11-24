This patch outputs four buttons at the right side of window titlebar to control window state by mouse left-click.
If FontAwesome (http://https://fontawesome.com) is installed, it outputs symbols 0xF2D1,0xF2D2,0xF2D0,0xF410, otherwise buttons are 
represented by default font text [_][o][O][X]. Left click on the buttons generates mouse event button11-button14 
that can be bound to a desired action in the i3 config file, e.g.:

bindsym button11 move scratchpad
bindsym button12 floating toggle
bindsym button13 fullscreen toggle
bindsym button14 kill

Thus, one can hide (move to scratchpad), toggle floating and fullscreen modes and close window by mouse left-click.

Patch is tested for i3 version 4.18.1 - 4.19.
