[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/MjLLqDcN)
# HW1
## W1L2 In-Class Activity

Put your notes from the W1L2 (Thurs, Jan 9) in-class activity here.

## Devlog
Prompt: Include the HW1 break-down exercise you wrote during the Week 1 - Lecture 2 (Jan 9) in-class activity (above). If you did not attend and perform this activity, review the lecture slides and write your own plan for how you believe HW1 should be built. If your initially proposed plan turned out significantly different than the activity answers given by Prof Reid, you may want to note what was different. Then, write about how the plan you wrote in the break-down connects to the code you wrote. Cite specific class names and method names in the code and GameObjects in your Unity Scene.


Write your Devlog here!

HW1 Breakdown: 
Objects:
1. UI
- Seeds planted shows how many seeds the player has planted
- Seeds remaining shows how many seeds the player has available
2. Player
- Movement with the WASD keys
- Player can plant plants with space bar
- Planting seeds effects the UI; seeds planted increments while seeds remaining decrements
- The player cannot plant seeds after they have used all of them
- Has a bunny sprite to represent player
- Player can still move even if no seeds remain
3. Plants
- Has a plant sprite to represent plant
- The plant appears in the front of player layer when planted 
- The plant has no physics or movement, unlike the player

This breakdown helped me complete HW 1 more easily. In the exercise file, I got two scripts Player and PlantCountUI. Thanks to the breakdown, I knew what I should code in the Player script, including updating the Player's movement using Input.GetKey and KeyCode WASD. Also, thanks to the breakdown, I knew I would need to write an extra line of code to use the spacebar for plant seeds. Prof. Reid helped me realize the difference in GetKey and GetKeyDown for the spacebar to avoid overlayering when planting seeds. The breakdown for UI helped me know what I needed to do next in PlantCountUI, and how I would update it in the Player script. I used _plantCountUI.UpdateSeeds to refer to the PlantCountUI script and called UpdateSeeds to run after each plant spawned. Thanks to the slides in class, I knew I needed to create a Prefab for the plant as a gameobject that is added multiple times and write code to spawn it when the spacebar is pressed, I used Instantiate in PlantSeed() to do this. In the sample game that Prof gave us, I noticed how the plant spawns on top of the player, and so I adjusted the layer in Unity for the plant object.


## Open-Source Assets
If you added any other outside assets, list them here!
- [Sprout Lands sprite asset pack](https://cupnooble.itch.io/sprout-lands-asset-pack) - character and item sprites
