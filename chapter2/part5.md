# First Video Game - Part 5 * EXTRA CREDIT *

This is an **extra credit part** worth extra 20% of your grade. If you do not wish to complete it, navigate to the assignment part of this chapter.

##

We already have a working scene with coin collection system. In this part, let's create a main menu and a mechanism that will end the game when all the coins are collected by the player.


## Create a new scene

File -> New Scene

![enter image description here](https://i.imgur.com/X782Z6i.png)

File -> Save, or use CTRL+S shortcut to save it. Name it "MenuScene" and save it in your "Scenes" directory.

## Design UI for the main menu

There are many ways in Unity to create UI and menus. In this tutorial we will be using the most popular and supported solution of Canvas.

### Add Game Title
In the Hierarchy tab, right click -> UI -> "Text - TextMeshPro"

![enter image description here](https://i.imgur.com/BdgDXSs.png)

Name it "GameTitle" and accept to import the TMP Essentials.

![enter image description here](https://i.imgur.com/zmpn8VS.png)

You can see the text that appeared in your scene. Do not edit the Canvas / UI asset from the scene tab. Instead, switch to the game tab that shows you exactly how the UI is displayed to the player.

Explore the "TextMeshPro - Text (UI)" component of the newly created "GameTitle" object.

![enter image description here](https://i.imgur.com/X0jpkAH.png)

Change the "Text Input" parameter to the name of your game - it might be "Coin collector 3D", "Tutorial Game" or any title you want! Edit the "Font Style" property to bold the font, and increase its size to 50.

Center the text by adjusting the "Rect Transform" component (reset position to 0, 0, 0). Increase its width and height to make sure it is displayed correctly.

![enter image description here](https://i.imgur.com/vKRR2c4.gif)

You can play with the position of your UI element by using the "Anchor Presets" modifying tool.

When you open the tool, hold ALT and SHIFT on your keyboard - this will tell the Unity to automatically set the position of our UI object to the selected one. The visual icons should be displaying a blue dot.
![enter image description here](https://i.imgur.com/CimYvx8.gif)

![enter image description here](https://i.imgur.com/G6jYErj.gif)

The text might still be a little bit off. To fix that, edit the "Alignment" property of the "TextMeshPro - Text (UI)" component.
![enter image description here](https://i.imgur.com/vblCGsj.png)


### Add author
1. Add another "Text - TextMeshPro" object, or duplicate your "GameTitle" object. Name it "Author".
2. Change its position and size so it is smaller than the title

![enter image description here](https://i.imgur.com/0z5QTYU.png)

I placed it on the top left corner.


### Change the background
There are also many ways in which we can add a background to the canvas. I will show two methods, you are free to choose one of them:

#### Method 1 - edit the Camera default background:
Click your "Main Camera" object and set the Environment -> Background Type property of a "Camera" component to "Solid Color".

![enter image description here](https://i.imgur.com/aGv8h8w.gif)

#### Method 2 - Add Canvas background object

Create another UI element. This time let's use an image. Right click -> UI -> Image.
Move it to a higher position in the hierarchy than *GameTitle* and *GameAuthor*. UI elements are rendered in order from the top to the bottom. We want the background to be rendered first, and then on top of it we want the text to be rendered.

![enter image description here](https://i.imgur.com/lp0Vmfn.gif)

And stretch it using the Anchor Presets dropdown (hold SHIFT + ALT and select the bottom-right icon). Change the color of the "Image" component.

![enter image description here](https://i.imgur.com/WJVea5X.gif)

### Add a start game button

Right click -> UI -> "Button - TextMeshPro".

![enter image description here](https://i.imgur.com/4cyAZAU.png)

Change its position and size, the same way as in the previous steps.

In the Hierarchy tab, collapse the Button element and click on its "Text (TMP)" child element.
![enter image description here](https://i.imgur.com/SbgRv17.gif)

Edit the "Text Input" parameter to for example "START".

![enter image description here](https://i.imgur.com/3IaZRpQ.png)

The visual aspect of our main menu is now ready.

![enter image description here](https://i.imgur.com/7hc6EwE.png)

## Create main menu script

Without a logic connected, the START button does not do anything. Let's create another script - "MainMenuController".
![enter image description here](https://i.imgur.com/co7Wxo2.png)

Edit the script:

    using UnityEngine;
	using UnityEngine.SceneManagement;

	public class MainMenuController : MonoBehaviour
	{
	    // Start is called once before the first execution of Update after the MonoBehaviour is created
	    void Start()
	    {
	        
	    }

	    // Update is called once per frame
	    void Update()
	    {
	        
	    }

	    public void StartGame()
	    {
	        SceneManager.LoadScene("GameScene");
	    }
	}


Create an empty object and name it "MainMenuController"
![enter image description here](https://i.imgur.com/79vrtFI.gif)

Drag and drop the "MainMenuController" script to the "MainMenuController" object.

![enter image description here](https://i.imgur.com/CIxMu9K.png)

The last step is to tell the button to execute the StartGame function defined in the script.

![enter image description here](https://i.imgur.com/GNCex0G.gif)

Play the game to test the start button. Once clicked, you should get an error message:
![enter image description here](https://i.imgur.com/hAT6KNX.png)

The reason of this error is that we did not tell Unity which scenes should be actually added to the project structure. To do that, click File -> "Build Profiles" to open the Build Profiles window.

Navigate to "Scene List" tab and remove the default "SampleScene" from the list.
Click "Add Open Scenes" button to add the currently open scene to the list.

![enter image description here](https://i.imgur.com/bMh5nf1.gif)

We need both the "MainMenuScene" and "GameScene" in this list, so once the "MainMenuScene" is added, open "GameScene" in your Unity Project tab, and in Build Profiles window add it as well.

![enter image description here](https://i.imgur.com/fUaOIqA.png)

![enter image description here](https://i.imgur.com/tTRfGCM.png)

##
[Next part (assignment)](https://github.com/mobaradev/unity-basics-to-vr-tutorial/blob/main/chapter2/part6.md)