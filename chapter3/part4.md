# Chapter 3 - From 2D Screen to VR - Part 4

In this chapter we are going to explore the build-in locomotion methods in the XR Rig. You do not need to use all of them (for the assignment *Controller walk* and *Teleportation* are required).

## Controller walk
It allows you to walk by using your left controller's thumbstick and is enabled by default.
You can find it in XR Origin (XR Rig) -> Locomotion -> Move.

![enter image description here](https://i.imgur.com/AlYYkle.png)

You can modify the speed of movement and enable strafe (walking sideways).

![enter image description here](https://i.imgur.com/JRoeZq3.png)

Use your left controller's thumbstick to walk in the virtual space.

![enter image description here](https://i.imgur.com/hxiySFx.png)

## Snap Turn rotation

Snap Turn rotation allows you to rotate your virtual world without changing your physical orientation.

![enter image description here](https://i.imgur.com/2x4sO1s.png)

You can modify the Turn Amount to a different value (default is 45 degrees), as well other parameters displayed in the "Snap Turn Provider" component.

![enter image description here](https://i.imgur.com/3mqtaIt.png)

Use your right controller's thumbstick to rotate horizontally.

![enter image description here](https://i.imgur.com/OBnc2lu.png)

## Teleportation

![enter image description here](https://i.imgur.com/fCmKKpD.gif)

![enter image description here](https://i.imgur.com/aovvCuX.png)

![enter image description here](https://i.imgur.com/3bRrlM3.gif)

![enter image description here](https://i.imgur.com/xoYvnEt.gif)

Use your right controller's thumbstick to point at your teleportation target. While pointing, you can tilt the thumbstick horizontally to adjust the orientation (if you checked the "Match Directional Input" in your object's "Teleportation Area" component).

![enter image description here](https://i.imgur.com/C7Eyxz6.png)


## Grab Move

The "Grab Move" locomotion is disabled by default.

![enter image description here](https://i.imgur.com/IrtCbfu.png)


![enter image description here](https://i.imgur.com/yXoIWuP.png)

To use this locomotion, press the grip button while pointing on any object nearby. Then move your controller (while still holding the grip button). Your character should move in the virtual space.

![enter image description here](https://i.imgur.com/DG33LPi.png)

## Grab Interactable objects

Create a cube (or any object). Add "XR Grab Interactable" component to it. A rigidbody component (that adds physics to the object) will be applied automatically.

![enter image description here](https://i.imgur.com/SbqFjSs.png)

To use this interaction, press the grip button while pointing at the object. Then move your controller (while still holding the grip button) - you should be able to hold and move/rotate the object.

![enter image description here](https://i.imgur.com/DG33LPi.png)
