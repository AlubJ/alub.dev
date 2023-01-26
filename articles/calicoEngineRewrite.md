# CalicoEngine Rewrite
![CalicoEngine Cover Photo](https://i.imgur.com/jCmLicb.png)

## What is CalicoEngine?
CalicoEngine is a 3d game engine that I wrote because I was bored. I wanted to work in 3d but didn't want to learn how to use Godot, Unity or Unreal, so instead I built the game engine on top of GameMaker.

For those who don't know, GameMaker is a primarily 2d game engine, but it does have *some* 3d functionality, only really abstracting the low-level OpenGL/DirectX code. GameMaker can build vertex buffers and push them to the GPU, and since GameMaker has support for shaders (thankfully), you can really do whatever rendering you would like. Want some lighting? Sure, why not? It's all possible in GameMaker (besides a few quirks).

The whole reason I wanted to make this game engine within GameMaker is because I felt more comfortable using GML over switching over to C++ or even just C.

## Why Restart?
The main CalicoEngine project file hasn't been updated in a while, not to mention the fact that I create new projects all the time. The biggest hurdle I hadn't jumped over at the time was external scripting, I wanted that figured out before I made a game, but in the end I just gave up... Until, I had found a scripting API called [Catspeak](https://github.com/katsaii/catspeak-lang), and all of my problems were solved! Brilliant!

I want to start from "scratch" because I'll be able to actually think about how the engine will load scenes, assets, and scripts, and figure out what functions to expose to the scripting API. Going back to the drawing board will hopefully allow me to think about each aspect of the game engine before pursuing a game.

## What's the Plan?
Well... I haven't exactly thought that far ahead. However, I am going to spend the next week or two directly planning the engine, and not touching the source code until I am confident what I plan will work.