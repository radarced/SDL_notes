SDL is dynamically linked meaning that u need the 
- declarations(.h files)
- compiled definitions(library -lSDL2 or SDL2.a)
- Library binaries(.dll files)
Library binaries on runtime is what the Operating system looks for to link the specified fucntion address to its import address ( the address is held inside the compiled defintions ) 