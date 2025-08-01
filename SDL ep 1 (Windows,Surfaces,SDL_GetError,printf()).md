## Window 
this is the viewport or the graphical viewport that you render rendering to;
[[Common Window Functions]]
## Surfaces
 [[SDL Surface]]

## SDL_GetError()

this SDL func is useful if anything inside SDL went wrong . any latest error within sdl can be tracked with this;

## prinf()

basically cout but u have to pass in the formats like %s %f for diffrent types like below
```
	printf("OOPSIES ? : %s\n:",SDL_GetError());
```
so %s is a string format and SDL_GetError() returns that and its put into the buffer and so forth;

