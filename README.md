# Mega65Toolkit
Somewhere to put all the bits and pieces that might be useful to others as I work on Mega65 development/


## Tile Conversion tools

https://github.com/MonstersGoBoom/AseSprite-scripts  -  Contains Tilemizer, an excellent Aseprite script for exporting full color mode chars, palettes and screen maps

## Floppyio.s

This file provides the tools to load files from d81 floppy without the need for the DOS ROM. It is very basic in functionality and comes with a kick macro for ease of use. It requires the use of $0200-$03ff for buffering data. Simply import the file and then call the Macro to load a file into memory anywhere up to $05FFFF. Note currently files should be loaded on 4K boundaries:

```
FLOPPY_LOAD($20000, "MYFILENAME")  
```
