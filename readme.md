An upgraded project of the so_long's project, cub3d shares the core concept using floodfill, handling key events such as pressing the standard WASD keys and presenting the image to the screen. However the difference between the so_long and the current project, cub3D, is the major conecpt of "raycasting"

What is raycasting? Raycasting is the heart of this project, normally you aren't able to see anything on the screen even if you are looking directly at the wall of the map. With raycasting, the line will collide with the wall, projecting the image of those pixel walls directly onto the screen, allowing us to actually see the game. These are usually done with calcuation and being able to get the color's value stored in our structures, as well as using the MiniLibx library to be able to code.

NOTE: Raycasting is not the same as raytracing! Raycasting is a fast semi-3D technique that works in realtime even on 4MHz graphical calculators, while raytracing is a realistic rendering technique that supports reflections and shadows in true 3D scenes.

Step 1: Validating The Map. While it's important to start the game, ensuring the map is valid is also another important thing to note. As stated in the subject's pdf, we need to ensure that the map is valid and if it's not, to exit the program without leaks.

Step 2: Calculating The Ray Direction The first step in the raycasting is to calculate the direction of the ray based on the player’s position and angle. We used dir_x and dir_y to store the player's direction with x and y coordinates respectively.

Step 3: Player's Movement We also need to add in player's movement to ensure that the player can move inside the map.

Step 4: Directional Check We needed to ensure that the map won't give us fish eye effects and the map details are projected correctly.

Step 5: Calculating Wall Height. The final step is to calculate the height of the wall based on the distance to the wall and the player’s view.

Step 6: Handling textures. In our project, we used .xpm files and used the .cub to find the path for our textures as well as the color of the floor and sky. It is also important that the textures, not matter how different each of them are in terms of width and/or height, should still be able to print inside the map.

Conclusion Cub3D is a fun project, and I hope this README make you understand better about how it works. Happy coding!
