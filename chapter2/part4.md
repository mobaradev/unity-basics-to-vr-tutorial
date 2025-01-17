# First Video Game - Part 4

In the previous part we created a script for a coin and we placed a bunch of coins on the map. When player touches it - the coin disappears. However without a game manager we cannot keep track of how many coins player collected.

## Game Manager
Create another script and call it "GameManager".

![enter image description here](https://i.imgur.com/duQMuat.png)

Create an empty gameobject "GameManager", and then drag and drop the "GameManager" script to it.

![enter image description here](https://i.imgur.com/qcBQUDg.gif)

Double click on the script file to open it in your code editor.

First, the manager should know how many coins are on the map. Add those two lines to the content of Start() function:

    int totalNumberOfCoins = FindObjectsByType<Coin>(FindObjectsSortMode.None).Length;  
	Debug.Log("Total number of coins to collect: " + totalNumberOfCoins);

Your entire GameManager.cs should look like that:
![enter image description here](https://i.imgur.com/540yNy7.png)

Play the game. A console message with number of coins should appear:
![enter image description here](https://i.imgur.com/gUQcdLB.png)

Let's update the script so it keeps track of already collected coins. When this value is equal to the total number of coins - the game should end.

    using UnityEngine;

	public class GameManager : MonoBehaviour
	{
	    public int CollectedCoins;
	    public int TotalNumberOfCoins;
	    
	    // Start is called once before the first execution of Update after the MonoBehaviour is created
	    void Start()
	    {
	        this.TotalNumberOfCoins = FindObjectsByType<Coin>(FindObjectsSortMode.None).Length;
	        Debug.Log("Total number of coins to collect: " + this.TotalNumberOfCoins);
	    }

	    // Update is called once per frame
	    void Update()
	    {
	        if (this.CollectedCoins >= this.TotalNumberOfCoins)
	        {
	            Debug.Log("You won!");
	            Debug.Break();
	        }
	    }

	    public void CoinCollected()
	    {
	        this.CollectedCoins = this.CollectedCoins + 1;
	        Debug.Log("Collected " + this.CollectedCoins + " / " + this.TotalNumberOfCoins + " coins.");
	    }
	}

But how the game manager will now if the coin was collected? The coin itself has to pass this information.
Let's quickly edit our **Coin.cs** OnTriggerEnter function. Replace it with the following code:

    private void OnTriggerEnter(Collider other)  
	{  
	  FindFirstObjectByType<GameManager>().GetComponent<GameManager>().CoinCollected();  
	  Destroy(this.gameObject);  
	}



Play the game again.

![enter image description here](https://i.imgur.com/MDdtHw6.png)

Collect all the coins and observe the console tab.
![enter image description here](https://i.imgur.com/huS1DWn.png)

Once you collected all the coins, you should see "You won!" message and the game should pause automatically thanks to the Debug.Break(); function we used in our GameManager script.

##
[Next part](https://github.com/mobaradev/unity-basics-to-vr-tutorial/blob/main/chapter2/part5.md)