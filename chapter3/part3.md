# Chapter 3 - From 2D Screen to VR - Part 3

This part is dedicated to discuss methods of testing your game for the VR device. You can utilize the Unity "XR Device Simulator" in your computer without access to any physical VR headset, or you can connect the headset to your computer and run your game directly in it.

## Unity XR Device Simulator
This simulator enables you to emulate the VR headset in your Unity3D editor with the use of your keyboard and mouse only. **USE IT ONLY WHEN YOU DO NOT HAVE ACCESS TO YOUR HEADSET**

Go to the Package Manager, locate the "XR Interaction Toolkit" package and in "Samples" tab, click the "Import" button next to the "XR Device Simulator".

![enter image description here](https://i.imgur.com/QtbBzkR.png)

In your project files, navigate to Assets -> Samples -> "XR Interaction Toolkit" -> "3.0.7" -> "XR Device Simulator".

Drag and drop the "XR Device Simulator" prefab to your scene.

![enter image description here](https://i.imgur.com/giCQjSV.png)

## Play it in your headset

### 1. Enable Developer Mode in your headset
To run and test your games in your Meta Quest headset, you first need to have the developer mode enabled.

Follow the steps from the meta developers website:
https://developers.meta.com/horizon/documentation/native/android/mobile-device-setup/

When you finished the developer mode setup, plug in the headset to your computer and make sure to allow the USB debugging in your headset.

![enter image description here](https://i.imgur.com/tOXdRiA.png)

### 2. Download "Meta Quest Link"
Go to the link: https://www.meta.com/quest/setup/?srsltid=AfmBOooa02paGycYOx38PZNnfclVMqe3BX83Ruf4C28CTVqQzld4Vqfi

Download & install the Meta Quest Link app.

Once opened, log in and go to the "Devices" tab. Add your headset there.
If you have a fast home Wi-Fi network you can connect it using "Air Link". This will not work correctly with slow networks (or shared like "eduroam").
Otherwise, link it through USB-C cable.

![enter image description here](https://i.imgur.com/ME6MT17.png)

Go to the "Settings' tab -> "General" tab and **allow Unknown sources**.
Then, also click the **"Set Meta Quest Link as active OpenXR Runtime"** button.

![enter image description here](https://i.imgur.com/e5zYa7j.png)


### 3. Start "Meta Quest Link" in your headset

Now your headset should be linked to your computer. Launch the link from your headset menu.

![enter image description here](../assets/images/ss14.gif)

***WARNING***
**You need either a fast USB-C cable OR a fast Wi-Fi network with both your headset and computer connected. This needs to be your home Wi-Fi network (you cannot use eduroam for that). If you have slower connection, the experience will be laggy and uncomfortable - in that case skip the Meta Quest Link part. You will have to build your app each time to play it - this is described in the part 5 of this chapter.**

### 4. Play your game from the Unity Editor

If you added the XR Device Simulator to your scene, **disable or remove** it when you play your game in the physical device. Otherwise, the game will not work correctly in your headset.

Click the Play button in your Unity editor.

![enter image description here](https://i.imgur.com/CkCzLh4.png)

The game should start in your headset. You should be able to look around and walk using your left controller's thumbstick.


## Build the game for your headset
If you cannot use the method above, you will have to build your app each time to play it - this is described in the part 5 of this chapter.