# Unity Scripts

## stretch.cs

This Unity script, named "stretch," adjusts the position, scale, and rotation of an object ("stretchcube")
based on the positions of two other objects ("cube1" and "cube2").

1. It calculates the center position between cube1 and cube2.
2. It sets the position of the stretchcube to the center position.
3. It calculates the distance between cube1 and cube2.
4. It sets the scale of the stretchcube along the axis connecting cube1 and cube2.
5. It rotates the stretchcube to align with the line between cube1 and cube2 using LookAt function.
6. Overall, this script effectively creates an object that stretches between two other objects and aligns itself with them.

Note: This script assumes that cube1, cube2, and stretchcube are assigned as public Transform variables in the Unity editor.
This also assumes that cube1 and cube2 have y-scale of 0, as the script only scales the stretchcube along the z-axis.

## movement.cs

This Unity script, named "Movement," provides WASD movement control for the object it's attached to, in the 2D XZ plane.

1. It detects horizontal and vertical input using the "Horizontal" and "Vertical" axes.
2. It translates the object horizontally and vertically based on the input and the frame time.

### Usage

Attach the "Movement" script to any GameObject you want to move using WASD controls in the XZ plane.

## README.md

This repository contains two Unity scripts:

1. `stretch.cs` - A script to create an object that stretches between two other objects and aligns itself with them.
2. `movement.cs` - A script providing WASD movement control for objects in the 2D XZ plane.

Feel free to use and modify these scripts in your Unity projects as needed.
