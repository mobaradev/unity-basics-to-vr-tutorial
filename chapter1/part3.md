# Unity3D Hello World - Part 3

In this part, we are going to utilize a player controller to walk, jump and look around!
To avoid coding and creating it from scratch, let's use an asset created by Unity Technologies that includes a ready to use First Person Controller.

Unity AssetStore offers a giant collection of packages, scripts, objects, textures, sounds and more.

## Import First Person Controller

Visit https://assetstore.unity.com/packages/essentials/starter-assets-firstperson-updates-in-new-charactercontroller-pa-196525
and import the package by first clicking "Add to My Assets" button
![enter image description here](https://i.imgur.com/WfK6jYi.png)

and then "Open in Unity".

A "Package Manager" window should appear in Unity3D.
Click download and then import button.
![enter image description here](https://i.imgur.com/Xk5QZwB.png)

If the dependencies warning window appears, click "Install/Upgrade":
![enter image description here](https://i.imgur.com/htQpOq1.png)

Import only the following directories (we don't need the other files included in this package):

 1. FirstPersonController
 2. InputSystem
 3. Mobile
 4. Settings

![enter image description here](https://i.imgur.com/gwkaEb7.png)

After this process is completed, you can see the "StarterAssets" directory is added to your assets:
![enter image description here](https://i.imgur.com/VU8RaoJ.png)

Go to StarterAssets/FirstPersonController/Prefabs and locate "PlayerCapsule" object.
Drag and drop it to the Hierarchy tab:[enter image description here](https://i.imgur.com/zBYesqi.png)

![enter image description here](https://i.imgur.com/NuCKzrZ.gif)

Now, you should be able to see it in the Game tab:
![enter image description here](https://i.imgur.com/o6NUBIH.png)

**If it is not visible from your camera perspective**, go to the Scene tab and change its position.
For example, set

 - "Main Camera" position as x = 0, y = 1, z = -10 and rotation 0, 0, 0.
 - "PlayerCapsule" position as x = 0, y = 0, z = 0 and rotation 0, 0, 0.


Play the game by clicking the "Play" button.

![enter image description here](https://i.imgur.com/q22AgID.png)

Use your keyboard WASD buttons to walk and space to jump!

*If it does not work, make sure to have the "Game" view active - mouse click on it and try again*

The capsule is pink because it does not have any material assigned. Any object without a material is by default rendered in this color. In this case we don't have to worry about it as we will use a First Person view, so the capsule will not be visible anyway but if you want you can apply a material to it.

In the Hierarchy tab, drag and drop "Main Camera" to "PlayerCameraRoot":
|  ![enter image description here](https://i.imgur.com/WJ1QqdG.png)|![enter image description here](https://i.imgur.com/Fu6bpQc.png)
|--|--|

Click on the "Main Camera" object and in the Inspector tab set its position to x = 0, y = 0, z = 0 and rotation = 0, 0, 0:
![enter image description here](https://i.imgur.com/hp4PwRD.png)

Play the game again. Now you should be able to control the player from its first person perspective!