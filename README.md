# Lunar lander (for HP Prime)

A lunar lander game that I am developing for the HP Prime graphing calculator. You can send this code into your calculator using the HP Connectivity Kit.

`lunar_lander.hpprgm` is the actual game so far, however it is still rather incomplete and the code started to get a tad messy, so I began development on the `vector-engine.hpprgm`, which is my rudimentary attempt to create a sort of game engine or framework to aid development.
(Disclaimer: I have never made a game engine before and I have no idea what I am doing.)

`terrain-test.hpprgm` is just a program I made while I was developing the random terrain generation for ease of testing.

I want to keep the scope of the 'engine' relatively small for now, so as not to overcomplicate this relatively simple game.
This would include rendering game objects and UI objects, some sort of camera functionality, taking inputs, applying basic physics, collision detection (but the collisions do not need to apply forces to objects yet), and maybe something else that I'm forgetting.
The point is, the engine should just be kept bare-bones for now, just enough to make this game, and it can be fleshed out afterwards.

## To do:
- [x] Make the lander rotate and do physics 
- [x] Random terrain generation with a little flat spot in the middle
- [x] Camera pan and zoom functionality
- [x] Limited fuel
- [ ] The engine, and cleaning of the code
- [ ] Collisions
- [ ] Game menu and stuff
- [ ] Smoothing of the follow camera, and implementation of zooming as the lander gets closer to the ground
