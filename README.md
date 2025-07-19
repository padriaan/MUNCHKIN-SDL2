# MUNCHKIN-SDL2
Remake of 38: Odyssey 2 K.C. Munchkin / Philips Videopac Munchkin
==================================================================

Remake of 38: Odyssey 2 K.C. Munchkin / Philips Videopac Munchkin
Originally released in 1981, programmed by Ed Averett.  


![Front_EU_resized](https://github.com/user-attachments/assets/1b689f52-96f4-491d-a65b-a9b82df61858) ![Front_US_resized](https://github.com/user-attachments/assets/0c20c7f1-c6b4-47c8-8a5d-9e2d7b18a3f0)


Created with SDL 2 in C.          
Requirements (devel + libs):
- SDL 2 
- SDL_mixer
- SDL_ttf
- Images (bmp), sounds (wav), Font (o2.ttf modified)

Created by Peter Adriaanse may 2025.
- Version 1.2.5  SDL 2 (Linux + Windows)

Press 1, Ctrl or Fire to start game.

Controls:  
- Joystick or cursor keys
- Use 8 to toggle full-screen on/off.  
- Esc to quit from game. Esc in start-screen to quit all.  
- Character keys for entering high score name. Return to complete.
  

![Title_screen_resized](https://github.com/user-attachments/assets/9cff1338-fbda-479c-b107-3fdea71ddf85)  ![In Game_resized](https://github.com/user-attachments/assets/6f2c1e94-6cd6-41b5-9e3c-008800284cb1)



Compile and link from source
-----------------------------
First install a SDL 2 development environment and C-compiler.

Linux:  
$  gcc -o munchkin munchkin.c -lSDL2 -lm -lSDL2_ttf -lSDL2_mixer

Windows (using MinGW):  
gcc -o munchkin.exe munchkin.c -Lc:\MinGW\include\SDL2 -lmingw32 -lSDL2main -lSDL2 -lSDL2_mixer -lSDL2_ttf

Run binary
------------
Download and extract the munchkin_all_in_one.zip  
OR  
Download src and data folders. Extract data.zip (to get data\images and data\sounds). Extract SDL2_ttf.zip (to get src\SDL2_ttf.dll)  

Execute in Windows:   
double-click munchkin.exe

Execute in Linux:   
$ export LD_LIBRARY_PATH=<folder where munchkin/src/linux_libs is located>  
$ cd src  
$ chmod 644 munchkin
$ ./munchkin

