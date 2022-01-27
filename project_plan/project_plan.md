# Project Plan 1st term Project Marco Winter
My project will a small first-person Unity game that explores the concepts of megastructures and “surreal movement”.   
My personal intention with this project is less about the presentation of a concrete story or academic theory, but about conquering my fears towards 3D and game engines.

## Visual Goals and Inspiration
My initial visual inspiration were these drawings by Kentaro Miura.

![Miura](imgs/01.png)  

Compared to his obvious influence M.C. Escher, Miura’s backgrounds are less ornamental and only feature simple geometry, which makes it a very suitable aesthetic for a beginner 3D project. I’ve started to create my first simple assets with ProBuilder inside of Unity, which can be easily stacked together like Lego bricks using ProGrids:

![Unity Demo](imgs/02.png)

The finished project will be a single seamless scene, but with **multiple areas** with a slightly different focus in geometry. While the first area features static stairs and archways, the latter ones might introduce additional geometry such as spheres and **animations of single enviromental elements**. Remeber these stairs?

![Potter Stairs](https://c.tenor.com/nTowZRm2PDAAAAAC/moving-stairs.gif)


I plan on using **multiple dynamic and volumetric lights** to make the structures appear much bigger than they actually are by only lighting certain segments at certain time. Instead of being textured, everything will remain black and white with a stark contrast, inspired by the works of [Anouk De Clercq](https://vimeo.com/user4524399) and Film Noire. 

![Volumetric Lighting](https://d3a2gvihmbqfjo.cloudfront.net/8f/8faf0349a0a1ce4e21377b8d4e2d7706/8faf0349a0a1ce4e21377b8d4e2d7706.png)  

I’m still unsure whether I should try for a **hand-drawn look using shaders** or not, but I’ll definitely try it out at some point.

## Game Mechanics and Player Motivation
This initial idea was in many ways very crude. Not only did I want to throw the players into an almost pitch black and illogical environment, but I also insisted to forgo and notion of game design or player guidance.   
Now that I incubated this idea for a while, I’ve come the conclusion that this would be way too depressing and also not all that interesting beyond a handful of screenshots.   

One of my initial ideas was also to include some sort of **gravity switching mechanic** since gravity is often relative in Miura’s and Escher’s artworks. Due to [this inspiring tutorial series by Jasper Flick](https://catlikecoding.com/unity/tutorials/movement/), I’ve decided to turn this into a major focus of the project. I’ll basically marry the edgy aesthetic with Super Mario Galaxy in first-person:

![Mario](https://catlikecoding.com/unity/tutorials/movement/complex-gravity/gravity-planes/gravity-range-scene.png)  

This might sound like an unlikely pair, but I think it precisely that can be interesting. This kind of “surreal movement” alone should provide some intrinsic motivation for the player and strengthen the strange atmosphere.   

To encourage the usage of these movement options even more, I’d like to **visualize the path taken by the player with a red trail of lights**. I could use Unity trail renderer for that, but even without it, it should be a feasible, though I’m afraid that a huge number of dynamic lights might crush the performance. In that case, I’d just use a red thread instead. 

![Trail Renderer](https://docs.unity3d.com/540/Documentation/uploads/Main/TrailRendererWindow.png)

With this feature, the player will be able to retrace her own crazy moves when looking back and it should make navigation as a whole a bit easier, while adding a touch of color to the monochromatic world.   

Going further with this idea of breaking up all the doom and gloom, I’d like to imply a **subtle love story** by having another single-colored light besides the player in the world. To tie this theme in with the weird movement,  I thought it might be nice to fade in 2D text at certain points in the game that relates the environment to relationships in some way. Which, of course would be quite corny, for example when the first quote after the first gravity shift would about how important it is to change your perspective once in a while…  
I’m not too sure on this one, but I like the idea of tying all everything together like this with a little contrast against the initial bleakness.

## Worst Case
- A single developed area
- Functional player movement
- A single showcase of gravity-switching
- Visualization of the path taken by the player (a red thread without shadows)
- A technical setup for a playable prototype

## Best Case
- Two or more areas
- Two or more instances of gravity-switiching
- Animated environments
- A lighting setup consisting of
    1. Dynamaic lighting
    2. Volumetric lighting
    3. Animated lights
- Playtime of about three to five minutes
- A visually more developed version of the player-trail (a glowing thread, a particle thread, a series of activa )
- Standalone application

## Nice to Have
- A shader setup for a hand-drawn look
- Self-made music and sound effects
- A dramaturgy consisting of
    1. A introductory area
    2. A clear endpoint
    3. A 2D text commentary on the different parts of the environment
    4. A blue light that guides the player in a very subtle way
- A web-based version

## Time Plan
### January
Development of a small prototype which includes
 - A small environment
 - Player movement. 
### February
- 1st week: Look-Development: Shader and lighting setup for the prototype. 
- 2nd week: Final touches on the lighting and experimentation with the player-trail.
- 3rd week + 4th week: The creation of addional areas.
### March
Bugfixing, adding the corny commentary