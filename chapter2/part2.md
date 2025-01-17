# First Video Game - Part 2

In this part we are going to create a coin object with a spinning animation.

## Create a coin object
Out of all the 3D built-in shapes, a "Cylinder" seems like a good candidate as a base for a coin. It just needs to be scaled and rotated in a certain way.

![enter image description here](https://i.imgur.com/Siw9Hvz.gif)

Then create a gold "Coin" material and apply it to the object.
![enter image description here](https://i.imgur.com/Xbp8Q6T.png)

Rename the object from "Cylinder" to "Coin":
![enter image description here](https://i.imgur.com/kKpKpPV.gif)

## Add spinning animation

There are multiple ways to spin gameobjects. To avoid unecessary coding, let's use Unity Animation tool. Open it from Window -> Animation -> Animation or using CTRL+6 shortcut.
![enter image description here](https://i.imgur.com/yhK6BvR.png)

A new window should show up. It is a tab that you can attach to already existing panels. I like to place it next to the "Project" and "Console" tabs but you are free to place it wherever you prefer, or leave it as separate window.
![enter image description here](https://i.imgur.com/iOiAaxf.gif)

Click "Create" and save it as "CoinAnimation" in your Assets. You can create a dedicated directory for animations - the same way as we keep all the materials in "Materials" folder.

![enter image description here](https://i.imgur.com/h9AHW7Z.gif)

Set the Rotation.y property to 360.

![enter image description here](https://i.imgur.com/6S84I1V.png)

Click Animation play clip button and observe what is happening.

![enter image description here](https://i.imgur.com/RRdHdLu.gif)

The coin is spinning counter clockwise! How and why? We set the Rotation.y to 360 in a starting time point 0:00, however the ending point 1:00 is kept as Rotation.y = 0. Unity automatically calculates all the points in between - so for example the mid point 0:30 will get a value of 180.

![enter image description here](https://i.imgur.com/z3MSW7D.png)

If you want the coin to spin clockwise, set the starting point 0:00 to Rotation.y = 0 and the ending point 1:00 to Rotation.y = 360.

Play the game to confirm the animation is working correctly.

![enter image description here](https://i.imgur.com/MDdtHw6.png)

##
[Next part](https://github.com/mobaradev/unity-basics-to-vr-tutorial/blob/main/chapter2/part3.md)