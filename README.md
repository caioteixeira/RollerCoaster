# RollerCoaster
A RollerCoaster simulation program built with C(with some C++ features) and OpenGL, used a Catmul-Rom Spline to draw the track and orient the camera.

![PrintScreen](https://raw.githubusercontent.com/caioteixeira/RollerCoaster/master/RollerCoaster.JPG?token=AENzdLXMDDL9uMnguh5qhIXlVwpnDTIDks5WOmFjwA%3D%3D)

[Click to see a demo video on Youtube :)](https://youtu.be/Pp_YjTthn4M)

## Arguments
The program need one argument on command-line, it's a path for a file indicating the path for control point definition files. You can see an example on track.txt.


## How to Compile
###Windows (Visual Studio)
Just import the project on Visual Studio and compile it. :)


###Mac

For Mac OS X, you will also need the [pic](http://run.usc.edu/cs420-s14/assignments/assign1/pic_MacOS.zip) image library. 
Before you compile, you must install command-line utilities (make, gcc, etc.). 
On Mac OS X Lion or newer, install XCode from the Mac app store, then go to XCode, 
and use "Preferences/Download" to install the command line tools. In Mac OS X Snow Leopard or older, 
you must install Mac OS X Developer Tools from the Mac OS X DVD. 
The makefile assumes that the pic library locates one level above (i.e. if starter code == /Users/tom/code/assign2, then pic library should be in /Users/tom/code/pic). Please compile the pic library before compiling the code. Here is a sequence of commands that get everything compiled:

	> unzip pic_MacOS.zip
	> cd pic 
	> export CPPFLAGS=-I/opt/X11/include
	> make 
	> cd ..
	> cd assign2
	> make
	> ./assign2 track.txt
