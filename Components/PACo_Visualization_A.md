# PACo_Visualization_A

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://user-images.githubusercontent.com/35654198/235983311-adbd7a45-ebb0-4f9a-84a9-e2cbb49a9479.png)

Above, the two possible visualizations are shown: An "Elevation" and a "Line".

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Theme | Data | Input | Record | The theme to use. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization to use. | See the documention on cmp_Visualization below. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Vizualization
With visualization, the visualization of a border is meant.

There are three possible visualizations:
- Elevation
  - See screenshot above.
- Line
  - BorderThickness: 1
- None
