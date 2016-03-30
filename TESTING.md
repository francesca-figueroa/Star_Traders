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

todo

**User Acceptance Tests**

TESTING PLAYER MOVEMENT
1. Start the game using Unreal Engine.
2. Press and hold W for about a second. The ship should move upward whilst the key is held.
3. Press and hold D for about a second. The ship should move rightward whilst the key is held.
4. Press and hold S for about a second. The ship should move downward whilst the key is held.
5. Press and hold A for about a second. The ship should move leftward whilst the key is held.
6. Record if and in what relative direction the ship moved for steps 2-5. Record if it moved in a way not described in the respective steps.

The test is considered a success if:
	the ship moved in all the expected ways as described in the instructions.

The test is considered a failure if the above is not true.


TESTING CORRECT GRAPHICAL CONFIGURATION
1. Start the game using Unreal Engine.
2. Observe disks created in a hexagonal grid, spanning beyond the entire screen.
3. Record that this is present, or describe how it varies from the description in 2.
4. Restart the game.
5. Observe a star potentially being orbited by up to 3 planets.
6. Record the number of planets the star is being orbited by.
7. Repeat steps 4-6 until either you have recorded 10 times or you have seen stars with 0, 1, 2, and 3 planets orbiting them.

The test is considered a success if:
	the grid in step 2 was observed as described in the step,
	and all 4 configurations of planets were observed in step 7.

The test is considered a failure if either of the above conditions are not true.


TESTING CONVERTING RESOURCES TO MONEY AND TRADING MENUS
1. Start the game using Unreal Engine.
2. You should be able to see how much money you have in the top-right. Record this. !(top-right?)
3. Click a nearby star. Record if a menu appears, and what the title of the menu is. !(this isn't implemented, test instructions will vary based on actual implementation)
4. The menu should have a number of buttons, including BUY, SELL, and EXIT. Left-click the BUY button. Record if the menu is replaced with a different one, and the new menu's title.
5. The menu should show a number of different resources in the game. Select the top one, then BUY one instance of that resource. Record the name of the resouce you bought. Exit out from the menus until you return to a screen with no menus as in step 2. Record the money value as in step 2.
6. Click the same star again. Using the same menu, click the SELL button. The menu will change to a new menu, similar to the BUY menu, but the selection of available resources changed to just the resource you bought. Record if this is the case, and the menu's title.
7. Select the resource you bought, then SELL it. Exit from the menus, then record the money value.

This test is considered successful if:
	the tester was able to complete the tasks described in the instructions,
	the recorded titles of the menus are all different from each other, and describe their functionality sufficiently (i.e. the buy menu should be titled "BUY RESOURCES" or similar),
	the initial value recorded for money is greater than both the values recorded after, !(this is a gameplay decision we still need to make, regarding the sold value)
	and the value recorded after selling the resource is greater than when that resource was bought.

The test is considered a failure if either of the above conditions are not true.
