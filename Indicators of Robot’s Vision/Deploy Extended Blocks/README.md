Week 1) 4/1/2024 - 4/8/2024
---
# Unity Scripts

## stretch.cs

This Unity script adjusts the position, scale, and rotation of a game object (`stretchcube`)
based on the positions of two other game objects (`cube1` and `cube2`).

1. It calculates the center position between `cube1` and `cube2`.
2. It sets the position of the `stretchcube` to the center position.
3. It calculates the distance between `cube1` and `cube2`.
4. It sets the scale of the `stretchcube` along the axis connecting cube1 and cube2.
5. It rotates the stretchcube to align with the line between `cube1` and `cube2` using the LookAt function.

Overall, this script effectively creates an object that stretches between two other objects and aligns itself with them.

Note: This script assumes that `cube1`, `cube2`, and stretchcube are assigned as public Transform variables in the Unity editor.
This also assumes that `cube1` and `cube2` have y-scale of 0, as the script only scales the `stretchcube` along the z-axis.

## movement.cs (Bonus)

This Unity script provides WASD movement control for the object it's attached to, in the 2D XZ plane.

1. It detects horizontal and vertical input using the "Horizontal" and "Vertical" axes.
2. It translates the object horizontally and vertically based on the input and the frame time.
   
### Usage

1. Create 2 game objects, each as a child of an image target (used as `cube1` and `cube2`).
2. Create a third game object to use as the extended block (or `stretchcube`).
3. Attach the `stretch.cs` script to the `stretchcube`.
4. Drag and drop the cubes from the Hierarchy into the `stretch.cs` script component to define the `stretchcubes` references of `cube1` and `cube2`

(Bonus)
1. Attach the `movement.cs` script to any GameObject you want to move using WASD controls in the XZ plane.
If the RARE lab decides to expand the research to a moving robot that turns it's head, we can use this function to demonstrate how it's vision moves across the table.
