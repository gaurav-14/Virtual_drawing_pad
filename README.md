# Virtual-Drawing-Pad

A simple application of computer vision using OpenCV library in ubuntu 14.04 LTS. Also works in Ubuntu 16.04.

Installation Required:

1.  OS: Ubuntu 14.04 or 16.04 (Tested for these two)
2.  OpenCV Library: https://docs.opencv.org/2.4/doc/tutorials/introduction/linux_install/linux_install.html

Compile:
g++ -ggdb vdp.cpp -o obj `pkg-config --cflags --libs opencv`

run:
./obj

The program uses thresholding function to detect marker in its environment.Then centroid is
determined using moments of image. The value corresponding to pixel is changed giving desired color.

The program is able to do following:

1.  Size of detected marker can be increased while drawing, giving strokes of various width.
2.  Able to choose any color for drawing.
3.  Able to use eraser of variable size.
4.  Marker goes undetected if it is placed away from certain range from camera.
5.  Able to save the drawing.

Enjoy Drawing!
