#Anton's OpenGL 4 Tutorials book demo code#

This series of demos accompanies the e-book "Anton's OpenGL 4 Tutorials":
http://www.amazon.com/gp/product/B00LAMQYF2

Copyright Dr Anton Gerdelan, Trinity College Dublin, Ireland. June 2014.
email: anton at antongerdelan dot net

## Info ##

See "LICENCE.txt" for licence information.

For updated information about this demonstration code, see:
http://antongerdelan.net/opengl/book_info.html

There is also an example of code for "Hello Triangle" for OpenGL 2.1 for
reference

All of these examples were built with a 64-bit Xubuntu Linux machine, so there
are Makefiles for 64-bit linux. I'm also adding project files for 32-bit linux,
32-bit windows (GCC and Visual Studio), and 64-bit Apple OS X but this will take
a few days and I might introduce some bugs. Send me an e-mail for any queries or
requests here.

Anton Gerdelan, 2 July 2014.

# About this fork

This fork describes a simple setup on OS X to run the demo code using homebrew
to install the libraries. Each example directory contains a `Makefile_Brew.osx`
file which is a make file updated to use the dependencies as installed by Brew.
All the examples have been tested and run correctly.

If you find any problem, please open an issue on this fork or better fork this
repo and send a Pull Request!!!

###Installing GLEW and GLFW3
* brew install --universal glew
* brew install --universal glfw3

###Initial Repo Setup
* $ Clone this forked repo. This repo is adapted to run on OS X without any
  modifications on your part.
* Alternatively, you can also fork this repo and then clone your fork, if you
wish to make modifications.

###About Brew based Makefiles for OS X

The Makefiles for OS X have been adapted to link to GLEW and GLFW installed via
brew above, while generating the output executable in each example directory.

The adapated make file is:`Makefile_Brew.osx`.

###Running the first_test/main.cpp
* $ cd `path to your repo dir`
* $ cd first_test
* $ make -f Makefile_Brew.osx
* $ ./demo

###### will return for example:
Renderer: NVIDIA GeForce GT 650M OpenGL Engine

OpenGL version supported 4.1 NVIDIA-10.2.7 310.41.25f01

###Running all the other examples
* $ cd `path to your forked clone repo dir`
* $ make -f `path_to_example`
* $ make -f Makefile_Brew.osx
* $ ./<BIN_FILE_NAME_IN_MAKE_FILE>;;; to run the example
