Makefile is a file extension with no like ".formats" and this file basically acts like an automation for the compilation command process; most files look something like this:
```
#OBJS specifies which files to compile as part of the project
OBJS = 01_hello_SDL.cpp

#CC specifies which compiler we're using
CC = g++

#COMPILER_FLAGS specifies the additional compilation options we're using
# -w suppresses all warnings
COMPILER_FLAGS = -w

#LINKER_FLAGS specifies the libraries we're linking against
LINKER_FLAGS = -lSDL2

#OBJ_NAME specifies the name of our exectuable
OBJ_NAME = 01_hello_SDL

#This is the target that compiles our executable
all : $(OBJS)
$(CC) $(OBJS) $(COMPILER_FLAGS) $(LINKER_FLAGS) -o $(OBJ_NAME)

```
basically all u need to know is that you create variables which represent the specific tokens after all of this u can create your command and reference those tokens by $(variable) and command syntax is "cmd : $(OBJS)"; you first pass in your files that u want to compile and then all the other things;