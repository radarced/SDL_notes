- SDL_GetWindowSuraface(SDL_Surface* ptr) :
	this takes in a surface and then i believe it just returns the reference to the window surface so basically meaning changing the surface - > changing the windows image
- SDL_BlitSurface(SDL_Surface* sourceSurface ,NULL,SDL_Surface* DestSurface,NULL) :
	this takes the sourceSurface and copies it over the DestSurface so basically modifying the DestSurface and then putting in the back buffer;
- SDL_ConvertSurface(SDL_Surface* srcsrface,SDL_Surface* dstsrface, SDL_Format):
this converts the format of the surface to the dst surfaces format;
lets say srcsrf has format 24bitmap and dst 32bitmap if u were to call the BlitSurface func 
it would convert this everysingle time u render to the backbuffer;
-SDL_BlitScaled(SDL_Surface* srcsrface,SDL_Surface* dstsrface, SDL_Rect Stretched Surface) :
this scales the src srface to the dstsrface and i think this also converts the format;
	```
	SDL_Window* _Window = SDL_CreateWindow(); // just pretend
	SDL_Surface* WindowSurface = SDL_GetWindowSurface(_Window);
	SDL_Surface* Image = SDL_LoadBMP("LOLOLOL.bmp");

	SDL_BlitSurface(Image,NULL,WindowSurface,NULL); // i dont know what the 2nd and 4th args are ;
```