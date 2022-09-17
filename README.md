# Godot4-MixamoLibraries
Make reusable Mixamo animations libraries that can retarget other models in Godot 4

![Controller Screenshot](https://github.com/pemguin005/Godot4-MixamoLibraries/blob/main/Screenshots/MixamoLib.GIF)

## UPDATE
Adobe's terms of service 6.2.E state not to make datasets or databases from their content which this could be seen as. 
To respect their service, I am removing the animations libraries and leaving only the Bone Map.
Below is a new tutorial showing how to make your own probject libraries for your own individual games.
Perhaps we can make own community open library of open animations. If I create any, I will share them here.
Thanks for your understanding.

## Features

Mixamo bone map res file, that can aid in making your own reusable libraries.

## Requirements
- Godot 4.0.13 Alpha or newer
- The Mixamo Bone Map.res file included here.

# How to use Library files once you have them:

- Drop into Godot's filesystem any Mixamo rigged model, (Preferabley exported in the base Tpose)
- Double click the model the Re-import it
- Select the skeleton, and select the bone map drop down, and select the Mixamo Bone Map.
- Drop this character model into scene, right click it and select "Make local".
- Select their animation player, click Animation > Manage Animations > Load Library > and select a library.res

It's now mapped to the new character!

# How to create your own library files:

## 1. Steps on Mixamo
- Download the Ybot model, import into blender
- Use the YBot in Mixamo to download all the animations you want
- Use the default fbx for downlaods, "Without skin", and select 'in place' when possible.

## 2. Steps in Blender
- Import base YBot
- Import each animation fbx (in another collection for easy visiblity, and easy removal later).
- In the Animatino tab, change the view to the "Nonlinear animation player"
- Name the first animation, and click push down to add it to the base Ybot.

- In the Nonlinear animation player, hit the 'N' key, a menu will appear on the right.
- Click the small drop down to select an animation from another armature
- Press Space bar to play the animatinon, name its animation, click push down.
- Repeat until all armatures animations are named and pushed to the base armature.
- Delete all other animatinon armatures.
- Save, check scale, export as glb. placeholder materials to save space.

## 3. Steps in Godot
- Bring .GLB into Godot filesystem
- Re-import, click "Skeleton3d", bone map drop down, load mixamo bone map.res.
- Drop the .glb into the scene, transfom 0,0,0,
- Right click > Make Local, Save as scene.
- Go to animation player, (test if you want that it works).
- Click Animation > Manage Animations
- To the right of Global, click the save icon, save the library.

DONE library now exists and it can be used on any skeleton that's been mapped in Godot

![Controller Screenshot](https://github.com/pemguin005/Godot4-MixamoLibraries/blob/main/Screenshots/Screenshot.jpg)

## Tutorial

A quick demonstration followed by a more indepth tutorial on how to use these libraries.

https://youtu.be/cetPEHgmATA

## Background

Explanation and inspiration  originally from FinePointCGI. Additional info can be found in their video about troubleshooting skelelon remapping. This project was inspired entirely by this video.
https://www.youtube.com/watch?v=NBukd3NmK88

## Support

Support me by checking out my music at https://bonesinthewalls.bandcamp.com, https://open.spotify.com/artist/3eKiNBKa9Jel0Ev98hcZll?si=dX0koLvrSWarOkSMaEmbmg, or searching "Bones in the Walls" where ever you stream music.
