Week 2) 4/9/2024 - 4/16/2024
---
# Unity Script: ChangeModel

## Overview

The "ChangeModel" script in Unity facilitates switching between different models by enabling and disabling corresponding GameObjects.

## Features

- **NextDesign():** Switches to the next design in the sequence.
- **PreviousDesign():** Switches to the previous design in the sequence.
- **ChooseDesign(int design):** Allows selection of a specific design by passing its index.
- **DisplayDesign(int design):** Displays the specified design by activating its corresponding GameObject.
- **ToggleDesign(int CurrentDesign, int DesignToShow):** Determines whether to show or hide a particular design based on the current design number.
- **HideAllDesigns():** Hides all design GameObjects.

## Usage

1. Attach the script to a GameObject in your Unity scene.
2. Assign GameObjects representing different designs to the appropriate public fields in the inspector.
3. Optionally, assign a TextMeshProUGUI component to the "DesignTextComponent" field for displaying design information.
4. Call the provided methods to switch between designs as needed.

## Design Numbers and Corresponding Designs

- **0) Baseline:** Baseline design.
- **1) Eye Socket:** Eye socket design.
- **2) Near-Eye Blocks:** Design with blocks near the eye.
- **3) Glasses:** Design with glasses.
- **4) Near-Eye Hands:** Design with hands near the eye.
- **5) Extended Blocks:** Design with extended blocks.
- **6) Blocks at Task:** Design with blocks at the task.
- **7) Projected Lines:** Design with projected lines.
- **8) Diminished Environment:** Design with a diminished environment.
- **9) Dim Environment:** Design with a dim environment.

Feel free to customize the script and GameObjects to fit your specific project requirements.
