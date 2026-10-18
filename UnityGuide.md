
# Introduction
- This guide assumes you are familiar with the 2022 Unity Editor, if not return once you are.
- This guide was made by taking the Submerged Among Us map's Unity Project as an example. 

# Prerequisites
- You will need the Among Us base classes from the game to add to gameobjects, download the [AssemblyCSharp](./Assembly-CSharp.dll) file and place it in `Assets/Plugins`.
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
