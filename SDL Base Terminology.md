some idioms of SDL :

```
	SDL_Init(SDL_INIT_VIDEO) <-- returns -1 if could not initialize SDL;
	SDL_Quit(); <-- closes all subsytems of SDL;
```
- SDL_INIT is needed to use the sdl functions just include the <SDL.h> header wont do it;
- SDL_Quit() quits all subsystems meaning : any kind of sdl subsystems that u asked sdl  for u to give access will be closed there memory would be deallocated. this is best practice .i dont think that it really matters just ending the main func would also cleanup;
# Rendering Buffers;
SDL doesnt render ur draws directly to the screen it works like this - > theres a back buffer where your draws are stored in and then when the updateWindow() func is called or anything like that it gets drawn to the front buffer; <- this Also means that
u DO NOT call the updateWindow() after every backbuffer drawcall otherwise ur basically drawing one by one and then drawing ;