# DivineOS - Public Domain Operating System

![alt text](https://i.ytimg.com/vi/mivUzwc3Qv8/maxresdefault_live.jpg)

## Build Instructions

Work in progress.

## Background

TempleOS was originally created by Terry A. Davis. Due to his unfortunate passing, he is no longer maintaining this project.\
This repository aims to improve upon the last release by Terry (v5.03 2017 November 20th).\
We will try our best to conform to Terry's original design philosophies while attempting to attract a larger audience through various changes and upgrades.

## Commandments

- Eleventh commandment:   Thou shall not litter.
- Twelfth commandment:    "Don't shoot unarmed men on the crapper." [http://www.youtube.com/watch?v=8wGiJcq95Ug](https://web.archive.org/web/20170901022101/https://www.youtube.com/watch?v=8wGiJcq95Ug)
- Thirteenth commandment: No gore unless it looks fake.
- Fourteenth commandment: No pedophilia or child porn.
- Fifteenth commandment:  Don't eat rare meat with blood.
- Sixteenth commandment:  No wife beating.
- Seventeen commandment:  Do not swing from radio towers with one hand.
- Eighteenth commandment: Do not disturb.

## Additional Information

TempleOS is a 64 bit, non-preemptive multi-tasking, multi-cored, public domain, open source, ring-0-only, single address space, non-networked, PC operating system for recreational programming. The OS runs 8-bit ASCII with graphics in source code and has a 2D and 3D graphics library, which run at 640x480 VGA with 16 colors. Like most modern operating systems, it has keyboard and mouse support. It supports ISO 9660, FAT32 and RedSea file systems (the latter created by Davis) with support for file compression. Many of these specifications—such as the 640x480 resolution, 16 color display, and single audio voice—were instructed to him by God. It also included an original flight simulator, compiler, and kernel.

## Keyboard Shortcuts

### General
- <kbd>Esc</kbd> Save & Exit 
- <kbd>Shift</kbd>+<kbd>Esc</kbd> Abort	& Exit
- <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> Reboot 
- <kbd>Shift</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> Soft Reboot 
- <kbd>Ctrl</kbd>+<kbd>D</kbd> File Manager

### Editing
- <kbd>Ctrl</kbd>+<kbd>S</kbd> Save
- <kbd>Ctrl</kbd>+<kbd>A</kbd> Save As
- <kbd>Alt</kbd>+<kbd>Backspace</kbd> Undo
- <kbd>Ctrl</kbd>+<kbd>Y</kbd> Delete Line
- <kbd>Ctrl</kbd>+<kbd>←</kbd> Beginning of Line
- <kbd>Ctrl</kbd>+<kbd>→</kbd> End of Line
- <kbd>Ctrl</kbd>+<kbd>↑</kbd>, <kbd>Home</kbd> Top of Document
- <kbd>Ctrl</kbd>+<kbd>↓</kbd>, <kbd>End</kbd> Bottom of Document
- <kbd>Ctrl</kbd>+<kbd>G</kbd> Goto line number
- <kbd>Ctrl</kbd>+<kbd>F</kbd> Find/Replace
- <kbd>F3</kbd> Next Occurence of Search
- <kbd>Shift</kbd>+<kbd>F3</kbd> Previous Occurence of Search
- <kbd>Ctrl</kbd>+<kbd>T</kbd> Toggle DolDoc Render
- <kbd>F5</kbd> JIT Compile
  
### AutoComplete
- <kbd>Alt</kbd>+<kbd>A</kbd> AutoComplete ON 
- <kbd>Alt</kbd>+<kbd>Shift</kbd>+<kbd>A</kbd> AutoComplete OFF 

### Window Manager
- <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>N</kbd> Focus Next Task (Like Alt+Tab)
- <kbd>Ctrl</kbd>+<kbd>X</kbd> Kill Current Task (Like Alt+F4)
- <kbd>Alt</kbd>+<kbd>M</kbd> Maximize Task
- <kbd>Alt</kbd>+<kbd>V</kbd> Tile Tasks Vertically
- <kbd>Alt</kbd>+<kbd>H</kbd> Tile Tasks Horizontally\
If there is only a single task, both of the tiling shortcuts can be used to make a task take up the whole screen space.
- <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>T</kbd> New Terminal
- <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Esc</kbd> New Terminal\
(More to come!)

## Getting Started

So great, you've installed DivineOS onto your machine, now what?

#### Take Tour (Y/N)?
This can get pretty annoying on every boot.
Edit Once.HC.Z to fix this.
```c
Ed("Once.HC.Z");
```
Remove the lines following `TipOfDay;`, up until the last `break;`

#### Personal Notes
Do <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>M</kbd> to open up a scratchpad for notes. This can be useful when working on a project
or using as a todo list. See `::/Demo/AcctExample/PersonalNotes.DD.Z`.

#### Disable the top border flashing and scrolling
This can also get annoying at times. To do this, you will have to edit 2 files.\
Firstly, Edit `::/Adam/DolDoc/DocTerm.HC.Z`. Go to line 30 using <kbd>Ctrl</kbd>+<kbd>G</kbd>. Remove `...` and `,SCX=15`. This stops the scrolling terminal title.\
Then go to line 35. Remove both `$BK,1$` and `$BK,0$`. This stops MENU from flashing.\
The second file is `::/Adam/DolDoc/DocEd.HC.Z`. Go to lines 105 and 113 and remove the same code as above.\
Do a Soft Reboot <kbd>Shift</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> to recompile.
#### Reading
Read `::/Doc/GuideLines.DD.Z` for a quick rundown on how the files are setup.

##### HolyC
For HolyC, read the HolyC DolDoc, and then get started on the Demo Index (both are in the help menu, accessible by <kbd>F1</kbd>).

## TODO

* [ ] Add build instructions
* [ ] Add supplementary discs
* [ ] Create a dedicated webite to host the code in RedSea format, with an online code viewer (this might require a modified git or svn to enable creating diffs for RedSea format)
