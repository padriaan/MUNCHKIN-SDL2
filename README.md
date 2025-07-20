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

Press 1, Ctrl, Enter or Joystick Fire to start game.  
Escape key of Joystick Home or Menu button to quit / go back.  

Controls:  
- Joystick or cursor keys  
- Use key 8 to toggle full-screen on/off.  
- Character keys for entering high score name. Return to complete.  
  
![select_game_resized](https://github.com/user-attachments/assets/957c0231-7fc6-49f1-904b-76481d822abd)

![menu_screen_resized](https://github.com/user-attachments/assets/71f2d285-f14d-4be5-9008-ad8abc0191ed)

![arcade_mode2_resized](https://github.com/user-attachments/assets/0ed3aef2-1a1c-41eb-a150-b2a77bbe5bb9)

![99_pills_resized](https://github.com/user-attachments/assets/52aafb54-82ed-4849-a07c-e17bf4accbb0)

![intermission1_resized](https://github.com/user-attachments/assets/9b0577c3-78ab-4718-a6ac-d6e164ca7c3c)

![intermission2_resized](https://github.com/user-attachments/assets/c8886bda-0f8c-47c1-bf4e-469927caee99)



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

