# PintoK_PutnamJ

## General Game Description

Hello and welcome to the Legally Distinct Cooking Game!

* The objective of this game is to complete all 5 dishes (Eggs and Toast, Fruit Medley, Vegetable Sandwich, Fruit Salad, and Hearty Breakfast) by combining 5 ingredients (apple, orange, bread, carrot, and egg) in the proper combinations for each dish.
* By grabbing and dropping the ingredients into the water of the cooking pot, ingredients will be added to a list appearing at the bottom of the Cookbook UI element floating above the user. Then, placing the lid on the cooking pot will start the cooking process, producing a dish (or a failure feedback noise) based on the included ingredients.
	* Successfully creating a new dish will reveal the dish's image on the UI Cookbook, play a success sound, and produce a brief spark effect above the pot before resetting the ingredients and pot.
	* Successfully creating a dish that has already been created will produce a different feedback sound and will reset the ingredients and pot.
	* Starting the cooking process without any included ingredients or an incorrect combination of them will produce a failure feedback sound and will reset the ingredients and pot. 
* Should the player wish to reset all ingredients currently in the pot in the event of a mistaken entry, they can simply grab the sink actor's faucet (gray protruding handle) to reset the ingredient list without starting the cooking process.
* Should the player wish to reset the positions of all the ingredients on the tables around them in the event of a dropped ingredient becoming unreachable, they can simply press the UI button labeled "Reset Ingredient Positions" on the Cookbook UI.
* To toggle viewing a hint on how to create a particular dish, the user may press the UI button labeled "Click Here for a Hint" below any of the dish images. Clicking the button again will reset the hint text. 
* Once the player has completed all 5 dishes in the Cookbook, they will be rewarded with a win sound, some text will appear on the Cookbook UI to indicate victory, and the cooking pot and lid will turn gold. The game can still be played in a "free mode" of sorts, but no new dishes can be created.

## Game Controls

* Interact with UI Button Elements
	* Using the RIGHT touch controller, the player may hover the casted ray from the controller over the button they wish to click on the Cookbook UI and use the shoulder (trigger) button to select UI elements.
* Grab Ingredients and Cooking Pot Lid
	* Using EITHER touch controller, the player may overlap their controller with the actor's mesh and hold the appropriate touch controller's side (grip) button to pick up the actor. Releasing the grip button will drop the ingredients, causing them to simulate physics and fall to the floor. The cooking pot lid will simply remain in place when dropped. Ingredients can also be thrown by releasing the grip button while holding an ingredient during the arc of an arm movement.
* Placing Ingredients and Cooking Pot Lid into/onto the Cooking Pot Cauldron
	* Overlap the held actor with the water of the cooking pot to trigger the event to add the ingredient to the pot (in the case of an ingredient) or to begin the cooking process (in the case of the lid). The actor does not still have to be held (so ingredients can be tossed in) for the overlap to trigger.
* Triggering the Sink Faucet
	* Similar to grabbing the ingredients or cooking pot lid, overlap EITHER touch controller with the sink's faucet mesh and press the appropriate touch controller's side (grip) button to trigger the ingredient reset process. The faucet will not be picked up, as the grab event immediately releases the component from the player's grasp (it would be strange if the sink's faucet was detachable...).
* Teleportation Locomotion
	* Teleportation is handled using the default Unreal Engine 5 built-in teleport. Using the RIGHT touch controller, move the joystick to an "up" position and point the controller to where you want to teleport. An arc will be drawn to the destination for the teleportation and a glowing blue circle will be drawn on the floor if the location is valid. Release the controller's joystick to complete the teleport.
* Turning
	* Snap turning is handled using the default Unreal Engine 5 built-in turning system. Using the LEFT touch controller, move the joystick to a "left" or "right" position to undergo a "snap" teleport in the appropriate direction of approximately 30-45 degrees. 
