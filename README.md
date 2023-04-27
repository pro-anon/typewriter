Plays a typewriter key sound on every key press.

# Dependencies
- X11
- SDL2, SDL2_mixer `sudo pacman -S sdl2 sdl2_mixer`

I've tried it with Zig version 0.11.0-dev.2336+5b82b4004.

# Command to run
`zig run typewriter.zig -lc -lX11 -lSDL2 -lSDL2_mixer`

# Command to build
`zig build-exe typewriter.zig -lc -lX11 -lSDL2 -lSDL2_mixer`

## Ubuntu 20.04 focal notes:

On ubuntu you can install the edge version of zig by doing:

```
sudo snap install zig --edge --classic
```

Then after install the `-dev` packages in the dependencies list, you're going to have to do: 

```
zig build-exe typewriter.zig -I/usr/include/SDL2 -lc -lX11 -lSDL2 -lSDL2_mixer
```


[typewriter.webm](https://user-images.githubusercontent.com/97809837/232880773-818e0d7b-a59a-446e-b14b-18f133f5f6c2.webm)