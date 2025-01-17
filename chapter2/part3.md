# First Video Game - Part 3

In this part we are going to create a script for the coin that will remove a coin once its collected by a player.

## Coin script
Let's write our first script! Create a directory "Scripts" and in it create a new "MonoBehaviour Script".
Name it "Coin" and double click to open it in your code editor.

![enter image description here](https://i.imgur.com/jWWFQbO.gif)

Edit the content by adding the OnTriggerEnter function. You can copy and paste the entire code.

    using System;
	using UnityEngine;

	public class Coin : MonoBehaviour
	{
	    // Start is called once before the first execution of Update after the MonoBehaviour is created
	    void Start()
	    {
	        
	    }

	    // Update is called once per frame
	    void Update()
	    {
	        
	    }

	    private void OnTriggerEnter(Collider other)
	    {
		    Debug.Log("An object entered the coin trigger");
	        Destroy(this.gameObject);
	    }
	}

**What does it do?**
OnTriggerEnter is an event function that is executed if another object enters the area of this object (in this case it is our coin).
When that happens - it will display a console message "An object entered the coin trigger" and then it will destroy the coin object from the scene.

Drag and drop the script to the "Coin" gameobject.

![enter image description here](https://i.imgur.com/5m9KfaT.gif)

And set the the "Is Trigger" property of "Capsule Collider" component as true.

![enter image description here](https://i.imgur.com/gfn3Hb1.png)

Without it being set as trigger, the OnTriggerEnter event that we just defined in our script would never be called!

![enter image description here](https://i.imgur.com/MDdtHw6.png)

Play the game and walk to collect the coin.

![enter image description here](https://i.imgur.com/iGe1j22.gif)
![enter image description here](../assets/images/ss10.gif)

You can see the message appears in the console tab once the player touches the coin. Immediately after that, the coin is deleted from the scene.

## Coin Prefab
Let's add more coins to the scene! We could simply duplicate the gameobject, however that is not a good practice. Any future change would need to be applied to every single copy.
To solve that problem, let's utilize concept of prefabs.

Create "Prefabs" directory.
![enter image description here](https://i.imgur.com/4zzClYZ.png)

And drag and drop the "Coin" gameobject to it:
![enter image description here](https://i.imgur.com/YLWR9zy.gif)

You can see its color in the Hierarchy tab changed to blue. It represents an instance of a prefab.

Now we can easily and safely add more coins to the scene. Simply drag and drop the prefab from your Project tab to the scene! You can also duplicate them from the Hierarchy tab.

![enter image description here](https://i.imgur.com/NrP45Ck.gif)

##
[Next part](https://github.com/mobaradev/unity-basics-to-vr-tutorial/blob/main/chapter2/part4.md)