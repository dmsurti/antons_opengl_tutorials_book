# For OS X only with Homebrew
Please note that [$ means Terminal Prompt]

###Installing GLEW and GLFW3
* brew install --universal glew
* brew install --universal glfw3

###Initial Repo Setup
* $ Clone this repo forked from antons repo. This repo is adapted to run on OS
X without any modifications on your part.
[ex:https://github.com/dmsurti/antons_opengl_tutorials_book]
* Alternatively, you can also fork my repo and then clone your fork, if you
wish to make modifications.

###About Brew based Makefiles for OS X

The Makefiles for OS X have been adapted to link to GLEW and GLFW installed via
brew above, while generating the output executable in each example directory.

The adapated make file is:`Makefile_Brew.osx`.

###Running the first_test/main.cpp
* $ cd `path to your forked clone repo dir`
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
