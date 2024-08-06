# Lunar lander (for HP Prime)

A lunar lander game that I am developing for the HP Prime graphing calculator. It is by no means complete at this stage. You should be able to copy and paste the code into the HP Prime Virtual Calculator (although this is untested) or you can send it to a real HP Prime using the HP Connectivity Kit. It is recommended that you use a G2 HP Prime (identifiable by the little "G2" in a circle on the back) for its much greater processing speed. The program has only been tested on a G2.

Note that while collision detection now works, it is also so slow that on a G2 HP Prime it usually runs <10FPS. Optimisation is the next big goal for this project.

This repository contains three folders: `hp-programs`, `plaintext`, and `other-stuff`. The first includes the `.hpprgm` files of the code, the second simply contains `.txt` files that I have copied and pasted the code into from the HP Connectivity Kit. The final folder contains random `.txt` folders I made during testing and prototyping.

`engine_lander.hpprgm` is the actual main program, although it requires `vector_engine.hpprgm`, which is my rudimentary attempt to create a sort of game engine or framework to aid development.
(Disclaimer: I have never made a game engine before and I have no idea what I am doing.)

`lunar_lander.hpprgm`, found in `other-stuff` was my first incomplete attempt at making the game before I decided I would be better off making an 'engine' with functions.
`terrain_test.hpprgm` is just a program I made while I was developing the random terrain generation for ease of testing.
Likewise, `dictionary_test.hpprgm` is my attempt at implementing dictionaries (I kept it separate from the main engine because they aren't really necessary).

I want to keep the scope of the 'engine' relatively small for now, so as not to overcomplicate this relatively simple game.
This would include rendering game objects and UI objects, some sort of camera functionality, taking inputs, applying basic physics, collision detection (but the collisions do not need to apply forces to objects yet), and maybe something else that I'm forgetting.
The point is, the engine should just be kept bare-bones for now, just enough to make this game, and it can be fleshed out afterwards. Any 'extra' features can go in separate files, like `dictionary_test.hpprgm`.

## Requirements:
- Update your HP Prime to the latest firmware
- Make sure you download both `engine_lander.hpprgm` and `vector_engine.hpprgm`
- Probably definitely make sure you have a G2 Prime.
- Ensure it is set to degrees mode when running the programs!

## To do:
- [x] Make the lander rotate and do physics 
- [x] Random terrain generation with a little flat spot in the middle
- [x] Camera pan and zoom functionality
- [x] Limited fuel
- [ ] Proper deltatime for rotation and things
- [ ] The engine, and cleaning of the code
- [x] Collisions
- [ ] Optimisation
- [ ] Radians compatibility
- [ ] Game menu and stuff
- [ ] Smoothing of the follow camera, and implementation of zooming as the lander gets closer to the ground
