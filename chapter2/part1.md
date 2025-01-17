# First Video Game - Part 1

## Open your project
Use the project from the previous chapter. You can also create a new project but make sure to have the [First Person Character package](https://assetstore.unity.com/packages/essentials/starter-assets-firstperson-updates-in-new-charactercontroller-pa-196525) imported.

## Create a new scene


![enter image description here](https://i.imgur.com/Sb9eT1X.png)

The new scene should appear, however it is not saved automatically:
![enter image description here](https://i.imgur.com/TQNZvPo.png)

Click File -> Save, or use CTRL+S shortcut to save it. Name it "GameScene" and save it in "Scenes" directory.


## Add platform and first person controller



### Platform
3D Object -> Plane.
Change its transform position to x = 0, y = 0, z = 0 and increase its scale to x = 10, y = 1 and z = 5.
![enter image description here](https://i.imgur.com/1BcXN66.png)

### First Person Controller

Drag and drop "PlayerCapsule" to the scene and move "Main Camera" to "PlayerCameraRoot" object.

![enter image description here](https://i.imgur.com/OCvTIdG.gif)

And reset "Main Camera" transform component to make it represent Player's first person perspective:
![enter image description here](https://i.imgur.com/cVsqDEo.gif)

##
[Next part](https://github.com/mobaradev/unity-basics-to-vr-tutorial/blob/main/chapter2/part2.md)