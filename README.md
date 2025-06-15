# DailyBread-old

**I'm not UBF member now, so this program won't be updated (maybe forever).**

### Warning
**Since something changed in UBF DailyBread service, this program does not work currently.**  
(I'm not sure whether I'll fix the program, since I don't use this program currently and nobody around me uses this program...)

### About
(Unofficial) UBF DailyBread viewer for PC I wrote in 2016.
This program provides the following functions:
- Download a 'bread' at any date (by crawling [UBF Bible Service](http://bs.ubf.kr/))
- Write your thoughts about the bread
- Save the bread in your computer
- Export the bread as a text file

![Screenshot](Image.png)

This program has some bugs (ex. It doesn't parse the bread properly at some dates.),
and it is very heavy (since it has to pack whole python and tk stuffs inside itself).
I created this repository just for referring to my old program in the future.
I will not upgrade this program, but write a new version in other language (ex. C++) from scratch in the future.

### How to run
- Run ```DailyBread.py``` to run the code directly.
- You need python 2.X with Tkinter support. (Recommended: python >= 2.7, tk >= 8.0)
- You can use pypy, too.

### How to build
- I used [py2exe](http://www.py2exe.org/) to build a standalone executable (for Windows).
- To build the executable, run ```setup.py```, and copy the folder ```data``` to the target folder.
- I recommend you to apply the patch described in [this link](http://stackoverflow.com/questions/14975018/creating-single-exe-using-py2exe-for-a-tkinter-program).
- The standalone version was tested on Windows 7 32bit / Windows 10 64bit.
- ~~I'll move to PyInstaller, cx_Freeze, or Nuitka to enable building for multiple platforms.~~

### Unittest
You can run unittest by running ```python -m unittest discover``` inside the directory ```src```.  
