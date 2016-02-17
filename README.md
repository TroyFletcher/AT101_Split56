AT101 Split56 "GhettoDox"
=============

![Before and After](https://raw.githubusercontent.com/FletchINKy/AT101_Split56/master/before_after.png)

*Easy AVR Install instructions*

Put or otherwise copy the contents of the handwire.cfg and handwire_hardware.cfg files to easy AVR's config directory. You may need to modify your handwire_hardware.cfg file to reflect the appropriate pins you use on your teensy. Two of the columns experienced issues with my teens, so I moved them, making it a little harder to wire and less logical. 

Build log album: https://imgur.com/a/M6PMB


Physical Layer Layout
=====================

![Physical to logical matrix layout](https://raw.githubusercontent.com/FletchINKy/AT101_Split56/master/Config_Matrix_to_Physical.png)
![Matrix and layout](https://raw.githubusercontent.com/FletchINKy/AT101_Split56/master/plotting_AT101_dox_layout.png)
_Notes on the Physical Layout_

The presumption of the layout is that the top most keys in the thumb clusters (Alt
and FN2 in this case) are the most easily accessible secondary cluster keys for
your thumbs, and the long keys (FN, right Space) are where your thumbs rest. If the
bottom secondary key is easier to press for your thumbs and your ergos, swap Alt
for Space and FN2 for \|. Also keep in mind there are keys you'll press and hold
while reaching (FN2 for example) and keeping those higher will probably be more
comfortable.

#[GUI Layout on Keyboard-Layout-Editor.com](http://www.keyboard-layout-editor.com/#/gists/4ee859fd40c0fa56aad4)

    Layer 0
    
    `~  1!  2@  3#  4$  5% 6^         7&  8*  9(  0)  -_  =+ 
    Tab  Q   W   E   R   T            Y   U   I   O   P   [{  ]} 
    Ctrl A   S   D   F   G             H   J   K   L   ;:  '" 
    Shift Z   X   C   V   B              N   M   ,<  .>  /? 
                           Alt        FN2
                       Space  FN  Space \|

_Notes on Layer 0_

**Missing keys**
The default layer is missing Enter, Backspace, Right Shift, all Windows (GUI)
keys, all function keys, arrows, and the Home/End cluster. These have been given a
high priority on the first function layer (FN1), which means your thumb needs to be
quick on the FN1 key to maintain basic function. You may consider using a lighter
switch for that key.

Left Space is primarily for scrolling (space on a webpage scrolls down, Shift+space
scrolls up) when your right hand is already on the mouse. This might not be part of
your workflow, in which case, it was previously an App key.

    


  
    
    Layer 1

    Mply  F1  F2  F3  A+F4  F5  F6          F7  F8  F9   F10    F11 F12 
    Tab  Esc  FN3 EnterApp  T             Y   U   M4  M5    Play    Vol- Vol+
    Ctrl A+Tab Tab C+L A+F  A+G               Lf  Dn  Up    Rt     ;: Enter
    Shift Z    X  C+C  C+V   B               Del Bksp C+S+Tab C+Tab  /? 
                             Alt         FN2
                        Space  FN  A+Space  Mute

_Notes on Layer 1_

4 to Alt F4 seemed obvious since I don't use F4 for anything else

A to Alt+Tab as a quick switch in windows.

D to Ctrl+L evolved from Alt+D to get to the URL bar, but Ctrl+L is more universal and reliable in windows which chokes on Alts some times

F to Alt+F is to shortcut to the File menubar

G to Alt+G is a native shortcut within Siebel, probably not useful to many

C and V to Ctrl+C and V are easy shortcuts when you're already holding down FN

W to Function Layer 3 (FN3) is for mouse control and was selected because it was
comfortable to hold. You may prefer to swap it for E if your middle finger is
easier to hold here.

HJKL to arrow keys because Vim

N and M to Del and Backspace keep those keys near eachother and make Control on the left easier

< and > to Ctrl+Shift+Tab and Ctrl+Tab is about switching between browser tabs easily

i and o are macros to Ctrl+B,p (switch to prevous buffer in tmux) and Ctrl+B,Ctrl+o (switch panes and focus on new pane)

' to enter is trying to work around the muscle memory. It's not working so far.

Mply is the live macro playback, and was selected on a tenkeyless layout, which put
the function an ~ closer together. Not sure if it'll survive here or be moved.

Space to Alt+Space is to open the windows context menu

    Layer 2
    
    Mrec 1!  2@  3# 4$  5%  6^      7&   8*  9(   0) Conf BOOT
    M7  M1  M2  M3  W+R  M6          Y    U    I    O  PtSc C+A+Del W+L
    Ctrl A   S   F   D   G          Home PgDn PgUp End  ;:  Enter 
    Shift Z   X   C   V   B           N    M   C+PgUp C+PgDn /? 
                            Alt         FN2
                          App  FN   Space  \|

_Notes on Layer 2_

Mrec is the live macro playback, and was selected on a tenkeyless layout, which put
the function an ~ closer together. Not sure if it'll survive here or be moved.

Q is M1 which is a macro which prints my email address.

W is M2 which is \ESC,:w\ENTER, which saves in vim. It helps that it's W

E is M3 which is exec('''\CTRL(v)''')\ENTER, which runs the pasted block of code in
Python IDLE, which can't handle the newlines of a regular paste.

R is Win(GUI)+R to open a Run dialog in windows, which is one of the few things I
actually use the windows key for.

T is M6 which is [^\\,t]+\\,t which is a regex I repeat commonly and is annoying to
type out repeatedlly.

[ and ] are CTRL+ALT+Delete (which is hard to type on this layout), and Window+L to
lock your screen (The second and only other reason I use the windows key.

< and > become CTRL+Page Up and Down to flip between excel sheets easily. Depending
on which you use more, you might want to swap these with the same keys on layer 1
if you Excel more than you tab browse.

    Layer 3
    
     `~  1!  2@  3#  4$  5%  6^        7&  8*  9(  M14 Conf Boot
    Tab  Q  FN3  E   R   T            Y   U   I   O  PtSc [{  ]}
    Ctrl A   S   F   D   G           Mlf Mdn Mup Mrt MB1 MB2 
    Shift Z   X   C   V   B             N   M   ,<  .>  /? 
                            Alt         FN2
                          App  FN   Space  \|

_Notes on Layer 3_

Layer 3 is generally mouse control and less used macros.

HJKL have been changed to arrow keys for mouse movement with ; and ' being used for
left mouse and right mouse. The pinky is not ideal for many presses, so "I" might be
better if you use the mouse to click often. Also note, HJKL does not support common
diagonal movement without moving fingers from the home row. You might be more
familiar with a wasd to ijkl style layout.

Issues
======
*Enter key* is bugging me. There is room to weld on another switch holder from
the pieces of the plate I have left without increasing the footprint much, but I
might just need more practice. Logically, the extra key can be the phantom key
left of N. (which was originally intended to be a fourth key on the left thumb
cluster) Until then, my right pinky just falls off into the abyss like when you
go up the last step in a staircase, and think there is another step and your foot
falls straight through your perception of reality.  

*Right shift* missing is a bit odd reaching for ~ or !. I dropped it off without
worry given there was zero visible wear on my QFR's right shift.

*Caps Lock* has that silly divot between it and the A, and makes me reach
further. The profile of the key doesn't make turning it over much of a solution.
Might have to fill it in or chop the original enter key (same row/profile) down
and put it there.

The rotation of the left side is making my muscle memory for some "inside"
control functions harder. Mostly Cut and Undo. I might have to function key those
as I have Copy and Paste

Considering some kind of mouse-assist layer for common functions I need when my
right hand is on the mouse. Ideally F3 since it's so unused on the left side.
Stuff like Delete, Backspace, possibly arrows. I'm trying to keep a record of
whenever I have to take my hand off the mouse to press a key on the right side.
Which is somewhat easy because it's annoying for me to have to do.

Ergonomics Notes
================
Still figuring out the most at-rest position for everything. Both thumb clusters
need to move inward, particularly the left one, which I didn't realize was so far
over

*The FN switch is TOO tactile*I actually think the function key needs to be more worn out. I press it so much
I'm catching failures to press it.

After using [tins](http://i.imgur.com/aAzhRBe.jpg) to raise the angle of both sides, I found it quite comfortable
and only noticed wrist issues at the end of the day, but they were cumbersome to carry and kind of noisy, so I
tried taking them away and running them tented slightly against the laptop. Immediately the wrist issues increased,
so I'm going to find a way to [flat-pack](http://www.instructables.com/id/Laser-Cut-Phone-Stand-1/) or flip-out stands for both sides.
