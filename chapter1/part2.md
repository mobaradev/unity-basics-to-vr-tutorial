# Unity3D Hello World - Part 2

In this part, we are going to create a simple scene with a platform and some objects.

## Prepare the scene
In Project tab, go to Assets -> Scenes and open the SampleScene.

![enter image description here](https://i.imgur.com/9uELUe1.png)

### Create a Plane
In the Hierarchy tab, right click -> 3D Object -> Plane.
![enter image description here](https://i.imgur.com/ivAss2J.png)

The platform has been added to the scene.

In the Inspector tab, right click on Transform component -> Reset to reset its world position values to 0, 0, 0.
![enter image description here](https://i.imgur.com/AcLJ0cb.png)

Select the plane in the Scene tab and change tool to "Scale tool"
![enter image description here](https://i.imgur.com/EhaUXBQ.png)

Rescale the plane so it is larger (for example 5x3 units):
![enter image description here](https://i.imgur.com/042LQI5.png)

### Add additional objects

Add Cube to the scene:![enter image description here](https://i.imgur.com/ejXQ1T9.png)

Switch to "Scene" tab and examine built-in transform tools (move, rotate and scale):
![enter image description here](https://i.imgur.com/bMIfqQy.png)

Move:
![enter image description here](https://i.imgur.com/rWZ3G5Q.gif) 

Rotate:
![enter image description here](https://i.imgur.com/oL0h1mo.gif)

Scale:
![enter image description here](https://i.imgur.com/DdzWid9.gif)

Add a few more cubes with different position, rotation and scale.

![enter image description here](https://i.imgur.com/HvuFhOe.png)

Switch to the "Game" tab and click the Play button:
![enter image description here](https://i.imgur.com/BxFUN2y.png)

Now you can see your scene from the "Main Camera" object perspective:
![enter image description here](https://i.imgur.com/hD8pCgF.png)

You can modify your scene objects during the playmode but those changes will not be saved when you stop the game.

## Colors

Every visible object in the scene needs a material. The default material used is the gray/silver you see in your current scene.
To add some colors, we need to create our own custom materials.

In order to keep the project organized, let's create a folder and call it "Materials":
![enter image description here](https://i.imgur.com/xwY5k9q.gif)

Create a new material in it and name it "Material1":
![enter image description here](https://i.imgur.com/cAPKlo3.png)

Drag and drop it to scene object of your choice:
![enter image description here](https://i.imgur.com/4vVZfo1.gif)

You can see the color of the object changed. To modify the color, click the "Material1" file and look at the "Inspector" tab.

Edit the "Base Map" using the built-in color selection tool:
![enter image description here](https://i.imgur.com/waRA9U4.gif)

Apply different colors to all your cubes and the plane (platform).