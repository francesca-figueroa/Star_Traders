# Star Traders

**Who**

Isabella Figueroa : francesca-figueroa

Robert Ballard : robertBallard

Nicholas Pfeufer : NicholasPfeufer

Brandon Jacquez : baroquemyheart


**Vision Statement**

We strive to make games we would enjoy playing.

**Automated Tests**

Since the project is being made in Unreal Engine, the engine generates and provides a testing utility for the game within the provided IDE.

To access the testing utility, once the project is open within Unreal Engine, then Window -> Developer Tools -> Session Frontend. Switch the to Automation tab, then one can perform tests using the interface shown in the below screenshot.

![automated testing image](https://github.com/francesca-figueroa/Star_Traders/blob/master/automationTestingExample.PNG "Automated testing.")

**User Acceptance Tests**

Use Case ID: UC-1

Use Case Name: Testing Player Movement

Description: Player can properly move their character using the WASD keys.



Users: Players

Pre-conditions: Game is running.

Post-conditions: Player can move the ship.

1. Press and hold W for about a second.

	System Response: The ship should move upward whilst the key is held.

2. Press and hold D for about a second.

	System Response: The ship should move rightward whilst the key is held.

3. Press and hold S for about a second.

	System Response: The ship should move downward whilst the key is held.

4. Press and hold A for about a second.

	System Response: The ship should move leftward whilst the key is held.



Use Case ID: UC-2

Use Case Name: Testing Correct Graphical Configuration

Description: The world map loads correctly and various features are present.



Users: Players

Pre-conditions: Game is running.

Post-conditions: The game is showing the player everything it needs to be graphically.

1. Observe disks created in a hexagonal grid.

2. Observe a star with up to 3 planets orbiting it.

3. Restart the game repeatedly, observing that star until you have observed that 0, 1, 2, and 3 planets can appear.

	System Response: Each restart, the system will set a variable randomly, changing the number of planets that appear for that run.



Use Case ID: UC-3

Use Case Name: Converting Resources to Money and Trading Menu Functionality

Description: Player can use money and resources to buy and sell other resources.



Users: Players

Pre-conditions: Game is running.

Post-conditions: Player has obtained, then sold, a resource.

1. Observe that the game is showing your current money supply in the top-right.

2. Click a nearby star.

	System Response: A menu describing the planet and trade options will appear.

3. Click the BUY button.

	System Response: A new menu will replace the old one, showing a number of different resources corresponding to that planet and options to buy those resources.

4. Select the top resource, then buy one of that resource.

	System Response: An amount will be deducted from the player's money supply, and they'll gain one of that resource.

5. Leave the BUY menu, then click on the SELL button in the original menu for the planet.

	System Response: A new menu will replace the old one, showing the resources the player has and what they could get in money for those resources.

6. Sell the resource you bought.

	System Response: The player will lose that resource, but gain some amount of money (less than what they paid for the resource).



