FCEUX port for Blackberry Playbook  

FCEUX is a Nintendo Entertainment System and 'Famicom' emulator of the classic 8bit console of the 1980s. 
This project uses SDL, TouchControlOverlay and the native development kit to implement a basic SDL port of FCEUX.
Currently there are glitches with sprite rendering but it's playable.  Input layout needs more work for sure.

http://www.fceux.com

Thanks:  FCEUX developers! 
         Jeremy Nicholl for detailed and quick responses to questions and his TCO library, and for fixing the audio init glitch.
         
Default game startup:
Create a directory called z:/misc/nes/roms  and place an unzipped game call 'game.nes' it will auto start this if no commandline options are given.

         

Issues:

1. Sprite glitches , garbled sprites appear portions are mirrored ( suspect endian issues )
2. LUA not compiled in yet.
3. OpenGL support not ported to GLES i.e. sdl-opengl.cpp 


Todo:

1. game loader startup screen to select  images 
2. better key layout , maybe dpad support.
3. compile LUA support back in
4. OpenGL port to GLES ( so change GL_QUAD, begin-end sequences etc )
5. USB host joystick support, should be possible on 2.x release so we can use proper pads.
6. Bluetooth, Phone control ?
7. Network support ( it's compiled in but original source is broken I believe )
 
 
contact: trevor.nunes@gmail.com
 
 
 