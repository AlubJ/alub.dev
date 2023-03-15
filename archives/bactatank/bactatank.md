# BactaTank Classic
![BactaTankThumb](https://i.imgur.com/AF7uRe2.png)

BactaTank is a character creation tool for LEGO Star Wars The Complete Saga, LEGO Indiana Jones The Original Adventures, and LEGO Batman The Video Game. You can create your own custom characters by editing textures, materials, and replacing meshes.

# Quick Start
## Recommened Tools
* [Paint.NET](https://getpaint.net/) - An image editor
* [Blender](https://www.blender.org/download/) - For mesh replacements
* [HxD](https://mh-nexus.de/en/hxd/) - A hex editor (For advanced users)

## Prerequisites
Firstly, you need a copy of the game you are going to be modding, extracted. Please follow this guide [here](https://www.youtube.com/watch?v=_EQ3hPrh0V8) before proceeding.

Before attempting any custom mesh replacements you will need a copy of Blender 2.8 or greater with the BactaTank plugin installed. You can find the plugin located in the `plugin` folder. To install in Blender go to `Edit >> Preferences >> Add-ons >> Install` and select `ttgames-model-format.zip` and install. After installing check the box to enable the plugin.

# Creating a Character
## Loading a Character
To load a character into BactaTank, either use; a preset character (amazing character bases built by talented modders to make your mods easier to make) or a character you want to load. You can drag character files onto BactaTank to open them too!
![bt_homepage](https://i.imgur.com/hTliNuY.png)

## Character Attributes Panel
The character attributes panel shows all the attributes currently implemented within BactaTank that are either editable or just viewable. Here you can select items to be edited or disabled.

To disable meshes or to disable rendering layers, right click the induvidual items. You can hold down `Left Control` to show only one layer. To disable rendering of bones and locators, just right click the `Bones` or `Locators` dropdown.

![bt_characterAttributes](https://i.imgur.com/UIMNuUe.gif)

## Editing Textures
To edit textures, select a texture, and export it. You can edit it in Paint.NET and save it as a `.dds` file with compression levels at `DXT1`, `DXT3`, or `DXT5`. To replace a texture click the `Replace Texture` button and select a new `.dds` file.
![bt_textures](https://i.imgur.com/ZYgnZmo.png)

## Replacing Meshes
With `v0.1.0` comes the addition of mesh swapping, the act of taking an existing mesh from the same or different character, and reimporting it. You can also change the bone-linkage for each mesh making it easy to swap meshes.

To replace a mesh, click on the `Replace Mesh` button, and select a `.btank` file from either an exported mesh from BactaTank or an exported mesh from Blender.
![bt_meshes](https://i.imgur.com/AsgtIjr.png)

## Editing Materials
The rendering has been updated for `v0.1.0` to render the character as closely as possible to the game. New additions include cubemapped matierals and better specular highlighting. So that when editing materials, you can get a good preview of what it might look like in game.
![bt_materials](https://i.imgur.com/N3UPicU.png)

## Editing Locators
Locators are what the game uses to place items, shadows, or vfx in the right place. Locators are usually connected to a specific bone with a slight offset in position, rotation and scale. The locators are coloured in blue in the viewer.

Right now, `v0.1.0` can only *edit* the position of a locator, however, you can build entirely new locators with the Locator Builder.
![bt_locators](https://i.imgur.com/MNiUDYG.png)

## Viewable Attributes
Currently, layers and bones are only viewable in BactaTank, however BactaTank does provide you with offsets if you would like to edit these attributes manually. You can change which material is used by a mesh which is sort of layer editing, but since it's more of a mesh editing feature, it's in mesh editor and not the locator editor.

# Credits
This tool has been a long time in the making, and while I did most of the programming myself, I couldn't have done it without these amazing people.

**Development Help**
* **Javster101**
* **IsaMorphic**
* **Slucier**
* **Aaron**
* **Skulluse**
* **Bario The Weird**
* **Suso**

**Testing**
* **Suso**
* **Cheatster9000x**
* **Jacko**
* **JustNathan**
* **INGWAR**
* **Terminus**
* **Austin**
* **GavinWK**
* **thereallintman**
* **Vader18**
* **Tobias**
* **Cosine_Rave**