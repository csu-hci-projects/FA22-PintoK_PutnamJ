# PintoK_PutnamJ

## General Game Description

Hello and welcome to the Legally Distinct Ball Game!

* The objective of this game is to complete all 5 levels (0 through 4) by "painting" all the map tiles (gray, granite-like plots on the ground) in each level.
* This can be accomplished by simply rolling over them, which consumes a certain amount of "paint" that also functions as the player's health.
* Running into obstacles (pencil towers) will also drain some paint and will cause the player's death if the damage is greater than their remaining paint.
* Falling out of the level will also cause the player's death, subtracting one from their remaining lives, found just below the paint bar.
* The number of lives the player starts with per level is dependent on the selected difficulty, as is the amount of paint used when painting tiles and when hitting obstacles.
	* Easy difficulty starts with 8 lives and painting tiles and hitting obstacles only uses a small amount of paint.
	* Medium difficulty starts with 5 lives and painting tiles and hitting obstacles uses a moderate amount of paint.
	* Hard difficulty starts with only 3 lives and painting tiles and hitting obstacles uses a lot of paint.
* Paint may be restored by picking up "Paint Bucket" collectables, which refills a set amount of paint that scales based on difficulty (harder difficulty means less paint restored; paint restored = 150% / difficulty level).

## Main Menu Description
* To begin playing, simply select the "Play Game" button from the Main Menu. Gameplay will begin from the level saved in the previous game run.
* To change the level you'd like to play on, open the "Level Select" menu and select the level you'd like to start from. Note that you can only start from a level you've already "unlocked", by clearing the level before it. The next run of the game (using "Play Game") will begin from the selected level.
* Completing a level will also advance the saved level value, meaning you can quit at any time and the game will remember the last stage you were on.
* Players can find options to change the background music volume, sound effect volume, background music track, and difficulty level in the "Options" menu. These options are stored in the game's save file as well and will be remembered on the game's next run.
* Additionally, at the top of the Main Menu, players can find the top score they've earned so far on any level. Score is calculated in the following manner:
	* Depending on the player's difficulty, each "gold coin" collectable pickup in the world will increase the player's score for that level by a factor of 100 x difficulty level (1 for easy, 2 for medium, 3 for hard).
	* Depending on the player's difficulty, completing a level with a certain number of lives remaining will add an additional value to the total score, weighing harder difficulty's lives more heavily.
	* At the end of each level, score is counted and written to the game's save file as a high score if it exceeds the previous value.
* Finally, players may clear the data they have stored in the save file using the "Clear Save Data" button in the bottom-right corner of the Main Menu. This replaces the existing save data with a default version, re-locking all levels and resetting all options to their defaults. Some options (like the chosen song) will only change at the start of the next play session (by clicking "Play Game"). 

## Game Controls

* Move Forward/Backward
	* Using the W and S keys on a keyboard or moving a gamepad's left joystick up and down, the player can increase the ball's forward rotation, moving them forward when on the ground, or generating a spin-in-place effect when in the air.
* Move Left/Right
	* Using the A and D keys on a keyboard or moving a gamepad's left joystick left and right, the player can increase the ball's lateral rotation, moving them sideways when on the ground, or generating a spin-in-place effect when in the air.
* Look Up/Down
	* Moving the mouse up and down or a gamepad's right joystick up and down, the player can control their view perspective on the ball in the up and down directions.
* Look Left/Right
	* Using the Q and E keys, moving the mouse left and right, or moving a gamepad's right joystick left and right, the player can control their view perspective on the ball in the left and down directions.
* Increase Look Sensitivity
	* Using the Up Arrow key, Period key, or the Up button on a gamepad's D-pad, the user can increase the sensitivity of the "look" controls, without a maximum value. This value is not saved between levels or game runs.
* Decrease Look Sensitivity
	* Using the Down Arrow key, Comma key, or the Down button on a gamepad's D-pad, the user can decrease the sensitivity of the "look" controls, up to a minimum value of 0.1. This value is not saved between levels or game runs.
* Jump
	* Using the space bar key or the bottom face button on a gamepad, the player can perform a "jump" action. The longer the button is held (up to a maximum of 2 seconds, indicated by a "shutter click" sound), the higher the player's jump will be when the button is released. Jumps can only be performed after hitting the ground, where a paint splatter will form on the ground of the same material as the player's "paint". When the player is in the air, they cannot change their direction or velocity other than by using the "Stop" and "Sneak" commands. So, be sure you have the lateral velocity needed before leaving the ground!
* Stop
	* Using the 0 key, Left Ctrl key, or the top face button on a gamepad, the player can immediately remove all their lateral velocities, leaving only the vertical component.
* Sneak
	* Using the Left Shift key, or the right trigger on a gamepad, the player can immediately decrease all their lateral velocities, leaving only the vertical component untouched. Additionally, while this key is held, the player's movement torque gain is decreased, allowing for more precise movement control.
* Pause Game
	* During play of a level, players may use the 6 key, Tab key, or Special Right key on a gamepad to open the Pause Menu, allowing the player to temporarily stop play, return to the main menu, or quit the game completely.
* Start Game (Deprecated)
	* Originally, players would start playing the game by pressing the 5 key or the Special Left button on a gamepad, but this feature was later discarded in favor of a menu system, which was found to be far more intuitive. The input action remains, as per the requirements, but currently does nothing.
* Auto Complete Level (Developer Tool)
	* Using the Backslash key, the player may choose to automatically skip the current level and proceed to the next one. This is intended to be a feature only for development and testing purposes.