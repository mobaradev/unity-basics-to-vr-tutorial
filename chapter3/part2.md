# Chapter 3 - From 2D Screen to VR - Part 2

## Create a new scene

File -> New Scene

![enter image description here](https://i.imgur.com/Sb9eT1X.png)

The new scene should appear, however it is not saved automatically:
![enter image description here](https://i.imgur.com/TQNZvPo.png)

Click File -> Save, or use CTRL+S shortcut to save it. Name it "VRScene" and save it in your "Scenes" directory.

Open the "Build Profiles" window (File -> Build Profiles).

![enter image description here](https://i.imgur.com/zmKG63Z.png)

Add the "VRScene" to your scene list. Move it to the first place (marked as 0), so it is the first scene to open when the game starts.

![enter image description here](https://i.imgur.com/4GtUC5F.png)

## Add platform and XR Origin

### Platform
The same way as in the previous parts, add a plane to the scene (3D Object -> Plane).
Change its transform position to x = 0, y = 0, z = 0 and increase its scale to x = 10, y = 1 and z = 5.
![enter image description here](https://i.imgur.com/1BcXN66.png)


### XR Origin
In your project files, navigate to Assets -> Samples -> "XR Interaction Toolkit" -> "3.0.7" -> "Starter Assets" -> "Prefabs".
Drag and drop the "XR Origin" prefab to your scene.

![enter image description here](https://i.imgur.com/FbJuOFO.gif)

Since the "XR Origin" object already comes with the first person camera attached, delete the default "Main Camera" object.

![enter image description here](https://i.imgur.com/NPIbJW1.gif)

The controller is now ready.