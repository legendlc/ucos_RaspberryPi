# uCOS-II on Raspberry Pi

This is a very basic port of uCOS-II to Raspberry Pi 2b. The version of uCOS-II we have used is V2.52.  

## Contents of each fold

bsp：Board support package. Handle interrupt,uart and timer

build：Store obj files generated during compilation

h：Head files, here the physical addresses defined in "regs.h" may need to be changed if you are using the early version of raspberry pi.
init：Startup code

lib：Library for standard c and libc 

port：Porting code 

ucos：Source code of uCOS-II.Here we don't proive the source code, and you can get the code from http://www.micrium.com. Be careful with the CASE of the name of the file names.

usrApp：Entry function: main and a simple application


## How to make
First, you should put the source code of uCOS-II in the fold "ucos".

For Windows: Download the yagarto toolchain. Then you can make directly.
For Linux: Get the toolchain, You maybe need to rewrite the makefile according to the toolchain used.
