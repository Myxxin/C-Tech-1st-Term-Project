# Project Documentation

# 1st day - 6th of January - Getting back to Unity and first Probuilder Experiments

The first day I took back to unity.   
I did a little bit of research this week and decided that I'd use the Probuilder package to build the environments for my projects. Probuilder should be sufficient since I only need the most basic geometric shapes (and I don't have the time for another program anyways). I watched [this video tutorial](https://www.youtube.com/watch?v=YtzIXCKr8Wo&list=PLMUuuDyzvcZLwoSLUPjFcjSvookPWgLz8&index=3&t=873s), which was ok, and created my first "level". 

![demo level](imgs/01.png)

During this ordeal, I noticed that the navigation in Unity is still quite a hassle for me, so I read [this part of the manual.](https://docs.unity3d.com/Manual/SceneViewNavigation.html)

## 2nd day - 7th of January	- Further Probuilder Experiments and an Inspiring Tutorial

I returned to my level and played a bit more with the different Probuilder tools after reading the [Probuilder documentation](https://unity-technologies.github.io/procore-legacy-docs/probuilder/probuilder2-gh-pages/). During a break, I stumbled upon [this tutorial series on movement and gravitation by Jasper Flick](https://catlikecoding.com/unity/tutorials/movement/), which inspired me a lot. I've decided to include Super Mario Galaxy-esque movement in my project. I also came up with the basic "plot" and context for the project, which eases the gloominess of the initial idea a bit. I've written about that in [my project plan here.](../project_plan/project_plan.md) 

## 8th + 9th of January - The Pain and Joy of being a Probuilder

I started a new scene with the idea to try some of the shapes that I'd use in my project, but it quickly evolved into something a bit more serious. I tried to recreate the structure from this panel:

![Miura](../project_plan/imgs/01.png)

I still struggled with the more advanced Probuilder features a lot - the basics seem to be much more reliable for my needs. I installed Progrids and read [the manual](https://docs.unity3d.com/Packages/com.unity.progrids@3.0/manual/index.html) so that I can easily snap objects together. After I while, I decided that it'd be smart to build my own reusable assets that I could snap together like LEGO bricks. I still don't entirely understand the concept of prefabs, but I got it working for me. To build some of the more complex (for me) assets, I looked into the experimental Boolean features of Probuilder after watching [this tutorial](https://www.youtube.com/watch?v=SpQsbqxAK4I&list=PLMUuuDyzvcZLwoSLUPjFcjSvookPWgLz8&index=4&t=224s). They seemed to be exactly what I needed, but there's a reason that they're an experimental feature. Most of the time, they immediately crashed my project. In the other cases, they just created an empty game object. I'll stick to my Minecraft approach. In the end, I ended up with this:

![My Miura](../project_plan/imgs/02.png)

I'm quite happy with that tbh. I thought about using a shader to improve the visuals without looking into lighting just yet. I found this shader, which might prove useful to get very close to Miura’s drawings, in case I want that.

At this point, I'm confident that I can build the environment as long as I got a nice copy and paste asset-based workflow going.

## Interim  10th - 12th of January - Creating the Project Plan Presentation

For my project plan presentation, I generated a bunch of additional ideas and structered them in a more cohesive way.  
You can find the result [here.](../project_plan/project_plan.md)

## 15th + 16th + 17th of January - The Pain ~~and Joy~~ of being a Probuilder Pt. II; First Shader Experiments

When I returned to my scene, I noticed lots of texture glitching and other artifacts. The culprits were lots and lots of overlapping faces. I created my assets by merging multiple primitves together, but unforntunately Probuilder does not simplify the resulting new object. Everything simply get's glued together. After loosing lots of hair, I seemingly soved the issue by merging the faces that I want the keep, detaching said faces and merging the detached faces back into new object. 

I decided to play around with materials by [Julio Sillet](https://juliosillet.gumroad.com/), but I didn't really like the outcomes. Instead, I purchased this [manga shader](https://assetstore.unity.com/packages/vfx/shaders/unchi-manga-shader-8504). I played around it quite a bit and got some nice results. HOWEVER, the shader revealed further imperfections in my assets: 

![Shitty Assets](imgs/02.png)

There are simply too many random vertecies in my assets due to the merging approach and some of the interior faces were still left. I decided to scrap all the assets I've build so far and started from scratch. I hate my entire existence. 

Since I couldn't rely on merging multiple objects together anymore, I had to rely on transforming the Probuilder primitives. This wouldn't be that much of an issue if the most of the Probuilder features would actually work. For example, the "Fill Holes" functionality crashes my project 90% of the time. For the remaining 10% it does something completely unexpected or nothing at all. 

Honestly, I would not recommend Probuilder. After Orkun's introduction, I researched whether there is a similar tool in Unreal and found out that Probuilder is a less sophisticated imitation of Unreal's [Geometry Brush Actors.](https://docs.unrealengine.com/4.27/en-US/Basics/Actors/Brushes/) Welp, I guess there is always another project...

## Interim II 19th + 20th of January - Creating this Documentation
I've decided to not use the Wiki since I didn't find a way to easily access it inside of VS Code.

## 27th + 28th of January - Enough Assets (for now)
I've created all the assets I want for now without any overlapping faces etc. They might not look spectacular and there are lots of seemingly similar arches for slightly different uses. BUT THEY ARE MINE ASSETS AND I'M VERY PROUD:

<img src="imgs/03.png" width ="1000">

Except for the stupid pillar, they also look pretty good with my current shader settings. It's obviously not a very realistic look, but I like how the spikes on the bridge contrast so nicely for example. I'll see whether I'll stay with this look or not later, it all depends on the lighting.
  
<img src="imgs/04.png" width="500">

