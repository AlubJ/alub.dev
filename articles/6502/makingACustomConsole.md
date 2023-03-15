# Making a Virtual Console
![6502 Console](https://i.imgur.com/jbuofXd.png)

## How This Project Started
At first, I wanted to make an NES emulator from scratch, following a [tutorial series made by javidx9](https://www.youtube.com/watch?v=nViZg02IMQo&list=PLrOv9FMX8xJHqMvSGB_9G9nZZ_4IgteYf). I only finished the CPU portion of this console, and so I had a 6502 emulator that could run any 6502 program rom. I let the project collect dust for a while until I decided that I wanted to create my own custom virtual console with it.

## RAM Layout
I started out by laying out the RAM into sections. Since this console is entirely virtual, I can lay out the RAM however I want to. I started by defining the program rom to be between `$8000` and `$ffff`, which is about 8k. 

The next bit of RAM I defined was Video RAM. I wanted 256 1-bit characters, and a screen buffer that was 40x25 characters in size. I also wanted an addition colour palette with 32 colours defined that the screen buffer can use for the foreground and background colour of each cell. One character takes up 8 bytes of RAM, with 256 characters, the character table ends up being `$0800` bytes long. Each cell in the screen buffer is 2 bytes, one byte for the character, and one byte for the foreground and background colour. With 1000 cells total, the screen buffer takes up `$07d0` bytes of RAM. In total, the Video RAM takes up `$0fe0` bytes.

At the moment, the Video RAM is very simple, and I may eventually switch the characters for a tilemap and sprites, just like the NES.

## Picture Processing Unit
