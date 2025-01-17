# Chapter 3 - From 2D Screen to VR - Part 1

Similarly to the First Person Controller, let's import and utilize the already implemented interaction toolkit.

## Import XR Interaction Toolkit

Open Window -> Package Manager.

![enter image description here](https://i.imgur.com/tzLTkjO.png)

Select the "Unity Registry" tab and find "XR Interaction Toolkit". Install it.

![enter image description here](https://i.imgur.com/K7g4oXV.png)

Switch to "Samples" tab and import "Starter Assets".

![enter image description here](https://i.imgur.com/OEgjhQU.png)

If a project settings window shows up with a possible project validation issues, click "Fix" or "Fix All".

![enter image description here](https://i.imgur.com/yI8Aqb5.png)

## Configure XR plugins
Open the Project Settings window (Edit -> "Project Settings") and navigate to the "XR Plugin Management" tab.

![enter image description here](https://i.imgur.com/Ds8tt7Z.png)

With the "Desktop" tab selected, check the "Oculus" as the "Plug-in Provider".
![enter image description here](https://i.imgur.com/0SBQ2cW.png)

Switch to the Android tab and check the "Oculus" as well.

![enter image description here](https://i.imgur.com/XbHoq3C.png)

If you do not see the  "Android" tab, it is most likely because you haven't install Android support for your Unity3D. Close your Unity window, open Unity Hub -> Installs -> Unity 6 -> Add modules.
![enter image description here](https://i.imgur.com/EcB2gmt.png)

and make sure you have the "Android Build Support" installed:
![enter image description here](https://i.imgur.com/5F2FRfj.png)

Go to the "Project Validation" and check for any issues / errors.

![enter image description here](https://i.imgur.com/f0iu71f.png)

The "Screen SPace Ambient Occlusion render" issue can be ignored.

![enter image description here](https://i.imgur.com/pztmJEg.png)

If there are no other problems detected, the XR support is configured correctly in your project.
