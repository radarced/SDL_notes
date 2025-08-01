SDL_UpdateWindowSurface(SDL_Window* Windowptr);
this updates the window's image . So after youve done drawing your going to call this func to render all ur updates on to the screen;

SDL_CreateWindow(const char* title , int x ,int y , int width , int height , SDL_WINDOW_ENUM)
the last one is one that sdl gives u a bunch of options of what kind of window u want so 
for instance : 
- SDL_WINDOW_SHOWN <-- this makes sure window is shown " i dont exactly know what this means"
- SDL_WINDOW_RESIZABLE 
this fnc returns NULL if window could not be created else it returns a window ptr;