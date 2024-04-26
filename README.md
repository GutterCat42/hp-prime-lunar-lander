# Lunar lander (for HP Prime)

A lunar lander game that I am developing for the HP Prime graphing calculator. It is by no means complete at this stage. You can copy and paste the code into the HP Prime Virtual Calculator or you can send it to a real HP Prime using the HP Connectivity Kit.

This repository contains two folders: `hp-programs` and `plaintext`. The former includes the `.hpprgm` files of the code, and the latter simply contains `.txt` files that I have copied and pasted the code into from the HP Connectivity Kit.

`lunar_lander.hpprgm` is the actual game so far, however it is still rather incomplete and the code started to get a tad messy, so I began development on the `vector_engine.hpprgm`, which is my rudimentary attempt to create a sort of game engine or framework to aid development.
(Disclaimer: I have never made a game engine before and I have no idea what I am doing.)
`engine_lander.hpprgm` is my attempt to 'port' the work I had done on `lunar_lander.hpprgm` into my 'engine'.

`terrain_test.hpprgm` is just a program I made while I was developing the random terrain generation for ease of testing.
Likewise, `dictionary_test.hpprgm` is my attempt at implementing dictionaries (I kept it separate from the main engine because they aren't really necessary).

I want to keep the scope of the 'engine' relatively small for now, so as not to overcomplicate this relatively simple game.
This would include rendering game objects and UI objects, some sort of camera functionality, taking inputs, applying basic physics, collision detection (but the collisions do not need to apply forces to objects yet), and maybe something else that I'm forgetting.
The point is, the engine should just be kept bare-bones for now, just enough to make this game, and it can be fleshed out afterwards. Any 'extra' features can go in separate files, like `dictionary_test.hpprgm`.

## Requirements:
- Update your HP Prime to the latest firmware
- Ensure it is set to degrees mode when running the programs!

## To do:
(these things are implemented only in `lunar_lander.hpprgm` so far)
- [x] Make the lander rotate and do physics 
- [x] Random terrain generation with a little flat spot in the middle
- [x] Camera pan and zoom functionality
- [x] Limited fuel
- [ ] The engine, and cleaning of the code
- [ ] Collisions
- [ ] Game menu and stuff
- [ ] Smoothing of the follow camera, and implementation of zooming as the lander gets closer to the ground
