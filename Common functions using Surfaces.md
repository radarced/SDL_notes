- SDL_GetWindowSuraface(SDL_Surface* ptr) :
	this takes in a surface and then i believe it just returns the reference to the window surface so basically meaning changing the surface - > changing the windows image
- SDL_BlitSurface(SDL_Surface* sourceSurface ,NULL,SDL_Surface* DestSurface,NULL) :
	this takes the sourceSurface and copies it over the DestSurface so basically modifying the DestSurface and then putting in the back buffer;
	```
	SDL_Window* _Window = SDL_CreateWindow(); // just pretend
	SDL_Surface* WindowSurface = SDL_GetWindowSurface(_Window);
	SDL_Surface* Image = SDL_LoadBMP("LOLOLOL.bmp");

	SDL_BlitSurface(Image,NULL,WindowSurface,NULL); // i dont know what the 2nd and 4th args are ;
```