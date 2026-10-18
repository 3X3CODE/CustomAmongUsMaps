

# Introduction
- This guide assumes you are familiar with the 2022 Unity Editor, if not return once you are.
- This guide was made by taking the Submerged Among Us map's Unity Project as an example. 

# Prerequisites
- You will need the Among Us base classes from the game to add to gameobjects, download the AssemblyCSharp file and place it in `Assets/Plugins`.
- Download the required tools listed below.

# Tools
install the following unity packages, 
- [Powersprite Animator](https://powerhoof.itch.io/powerspriteanimator) (optional for more features, will be primarily focused on in this guide)
- [AssetBundle Browser](https://github.com/Unity-Technologies/AssetBundles-Browser) (follow the steps on the github repository)
- Text Mesh Pro
>[!NOTE]
>Install `.unitypackage` files by double clicking on them in the editor

# Folder Structure

- Assuming you have already created your unity project (follow the Unity Project setup step in the [main file](./ReadMe.md) if you haven't), open the `Assets`folder.
- The `Assets` folder will get messy quick as most packages use it for their own folders, so Create a new folder for your map specifically.
eg: 
```text
Assets/
├── MyCustomMap
└── PowerSpriteAnimator
```
- Everything related to your map should be in the folder created in the previous step
- Your Custom Map will feature one or more of the following, 
1. Map
2. Minigame
3. HudMap
4. ExileCutscene

* Create subfolders for each of those your map will have
eg:
```text
Assets/
└── MyCustomMap/
    └── Map
    └── Minigames
    └── HudMap
    └── ExileCutscene
```

- Now let's do a deep-dive on each of them
>[!NOTE]
>Click the links below to jump to wherever you desire!

<div align="center">
    
[Maps](#maps) &emsp;
[Minigames](#minigames) &emsp;
[HudMap](#hud-map) &emsp;
[ExileCutscene](#exile-cutscene)

</div>

<div align="center">
<h1>Maps</h1>
</div>

- This section will be focusing on the main map itself.

## Folder Structure and Setup

- You can further create more subfolders 
eg:
```text
Assets/
└── MyCustomMap/
    └── Map
        ├── Animations
        ├── Doors
        ├── Vents
        └──Textures
```

Animations :- map animations <br>
Doors :- Horizontal and Vertical door prefabs <br>
Vents:- Standard vent prefab and other configurations if any <br>
Textures :- All sprites/spritesheets of the map 

- It is recommended to have the .anim files in the `Animations` folder and the frames for the animations under a subfolder in the `Textures` folder.

- Make sure to keep things organized to prevent a hassle later on.

## Creating the Map Prefab

- The Map Prefab is the **most important** part of a Custom Map and the largest.
- The Map Prefab is instantiated by the game once you enter the game.

- Even here, having a good gameobject structure is a must, feel free to create additional objects to further organize items.

<h3>Rooms</h3>

- Room objects consist of the following, 
1. Background
2. Consoles
3. Animations

<h3>Colliders</h3>

- Colliders are a significant part of a custom map.

<div align="center">
<h1>Minigames</h1>
</div>
<div align="center">
<h1>Hud Map</h1>
</div>
<div align="center">
<h1>Exile Cutscene</h1>
</div>
