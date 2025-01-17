## Assignment
Submit a screenshot of your Unity3D with the "GameScene" open. **Include the entire Unity3D window** with all the panels (Hierarchy, Scene/Game, Project) visible.

*Example screenshot:*

![enter image description here](https://i.imgur.com/lO95uWB.png)



## Extra credits

### Extra credit 1 [+20%]
Complete the part 5 of this tutorial (UI and main menu). Submit a screenshot of your main menu - your author name should be visible somewhere in it. Feel free to change colors, font size, positions of UI elements - do not copy 1:1 from my example implementation.

*Example implementation:*
![enter image description here](https://i.imgur.com/cKQ8EFQ.png)


### Extra credit 2 [+5%]
*This extra credit requires you to complete the Extra credit 1 first.*

Currently when all the coins are collected, the game pauses. Change that, so the player is put back in the main menu.

**Hint:** Edit the GameManager script and use *SceneManager.LoadScene* (similarly as it is used in the MainMenuController).

Submit your modified GameManager.cs


### Extra credit 3 [+10%]
Add the UI text to your GameScene that would dynamically show the number of coins collected and the total numbers of coins to collect - for example "Coins: 3 / 10". Place it in the top-left or top-right corner of the screen.

*Example implementation:*
![enter image description here](https://i.imgur.com/yHKkfQs.gif)

**Hint:** Edit the GameManager script. Define a *public TextMeshProUGUI*, and modify the *CoinCollected* function to set the value. Don't forget to drag&drop your UI text element to the GameManager.

Submit your modified GameManager.cs