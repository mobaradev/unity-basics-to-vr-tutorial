# Chapter 3 - From 2D Screen to VR - Part 5

In this chapter we are going to build the game file. You will be able to share this file to other people!

## Switch build profile to Android

Open the Build Profiles window, navigate to the Android tab and you should be able to select your Quest headset as the "Run Device".

![enter image description here](https://i.imgur.com/B5uuo3P.gif)

### Build and run the game

Switch to "Android" tab. Click the "Refresh" button next to the "Run Device" field and select your headset there. If you can't find it, try to unlink/unplug and link/plug your headset back. Make sure you followed the instructions from the part 3 of this tutorial (*Meta Quest Link is set as active OpenXR Runtime*).

![enter image description here](https://i.imgur.com/X2MLo0k.png)

Click "Build and Run" button.

![enter image description here](https://i.imgur.com/nlrWEKU.gif)

If the "Unsupported Input Handling" warning window appears, you can safely ignore it by clicking "Yes".

![enter image description here](https://i.imgur.com/PL4rSGm.png)


![enter image description here](https://i.imgur.com/rS0vDfG.png)

The build process may take a while (even over 10 minutes depending on your CPU speed) and after its successfully completed, the game should start in your VR headset. The ".apk" file will be saved in your project folder.

If the game starts but you cannot look around, make sure you correctly followed the previous steps. The XR Device Simulator needs to be deleted from your scene and the "VRScene" should be first in your build scene list.
