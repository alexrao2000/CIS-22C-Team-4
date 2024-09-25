# CIS-22C-Team-4
Details: Here is where we will keep our code for the CIS 22C final group project. This project was part of contest which we entered as Team 4.

Project summary:
	Topic: Tablet convertible Laptops.
  
	Members: 
		Alex: File I/O 
		Andrew: Priority Queue
		Jasper: GUI
		Mohamed: Team Coordinator & Main
		Tin: Hash Tables
		Vu: BST Algorithms

### To Compile and run the program on Mac:

first install home-brew from [brew.sh](https://brew.sh) if you don't have it already.
then install two packages:
>brew install pkg-config

>brew install gtk


pkg-config manages the includes and libraries for the project

gtk is the graphics library the project uses

make sure install gtk2 and NOT gtk3

then use this command to compile the program (make sure you cd into the correct directory first)
>g++ \*.cpp -o program \`pkg-config --cflags gtk+-2.0\` \`pkg-config --libs gtk+-2.0\`

and then run it
>./program

#### Coming Soon:
For Mac users we will soon have a .app ready to download, no package installation required!

### For Windows:
Make sure you have GTK installed. Tested with GTK3.
Use a makefile, or copy the following into a .bat file:
~~~~
@echo off
  
set gtk_ver=gtk+-3.0
pkg-config %gtk_ver% --cflags --libs >tmp.txt
set /p pkg-info= <tmp.txt
del tmp.txt

rem echo %pkg-info%
g++ *.cpp -o program.exe -Wall %pkg-info%
pause
~~~~
and put it in the directory with your code.
