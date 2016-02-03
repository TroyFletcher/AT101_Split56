AT101_Split56
=============

*Easy AVR Install instructions*

Put or otherwise copy the contents of the handwire.cfg and handwire_hardware.cfg files to easy AVR's config directory. You may need to modify your handwire_hardware.cfg file to reflect the appropriate pins you use on your teensy. Two of the columns experienced issues with my teens, so I moved them, making it a little harder to wire and less logical. 

Build log album: https://imgur.com/a/M6PMB


Physical Layer Layout
=====================
    
    Layer 0
    
    Layer 1
    Mply  F1  F2  F3  A+F4  F5  F6          F7  F8  F9   F10    F11 F12 
    Tab  Esc  FN3 EnterApp  T             Y   U   M4  M5    Play    Vol- Vol+
    Ctrl A+Tab Tab C+L A+F  A+G               Lf  Dn  Up    Rt     ;: Enter
    Shift Z    X  C+C  C+V   B               Del Bksp C+S+Tab C+Tab  /? 
                             Alt        FN2
                           App  FN  Space  Mute
_Notes on Layer 1_

4 to Alt F4 seemed obvious since I don't use F4 for anything else

A to Alt+Tab as a quick switch in windows.

D to Ctrl+L evolved from Alt+D to get to the URL bar, but Ctrl+L is more universal and reliable in windows which chokes on Alts some times

F to Alt+F is to shortcut to the File menubar

G to Alt+G is a native shortcut within Siebel, probably not useful to many

C and V to Ctrl+C and V are easy shortcuts when you're already holding down FN

HJKL to arrow keys because Vim

N and M to Del and Backspace keep those keys near eachother and make Control on the left easier

< and > to Ctrl+Shift+Tab and Ctrl+Tab is about switching between browser tabs easily

i and o are macros to Ctrl+B,p (switch to prevous buffer in tmux) and Ctrl+B,Ctrl+o (switch panes and focus on new pane)

' to enter is trying to work around the muscle memory. It's not working so far.

    
    Layer 2
    MrecM11 M12 M13  4$  5%  6^          7&    8*    9(    0) Conf   BOOT 
     M7  M1  M2  M3  R   M6             Y     U     I     O   P C+A+Del W+L 
     Ctrl A   S   F   D   G              Home PgDn PgUp  End  ;: Alt 
     Shift Z   X   C   V   B               N   M  C+PgUp C+PgDn /? 
                            Alt        FN2
                          App  FN  Space  \|

_Notes on Layer 2_

Issues
======
*Enter key* is bugging me. There is room to weld on another switch holder from the pieces of the plate I have left without increasing the footprint much, but I might just need more practice. Logically, the extra key can be the phantom key left of N. (which was originally intended to be a fourth key on the left thumb cluster) Until then, my right pinky just falls off into the abyss like when you go up the last step in a staircase, and think there is another step and your foot falls straight through your perception of reality.  

*Right shift* missing is a bit odd reaching for ~ or !. I dropped it off without worry given there was zero visible wear on my QFR's right shift.

*Caps Lock* has that silly divot between it and the A, and makes me reach further. The profile of the key doesn't make turning it over much of a solution. Might have to fill it in or chop the original enter key (same row/profile) down and put it there.

The rotation of the left side is making my muscle memory for some "inside" control functions harder. Mostly Cut and Undo. I might have to function key those as I have Copy and Paste
