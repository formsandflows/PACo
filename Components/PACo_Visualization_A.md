# PACo_Visualization_A

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://github.com/formsandflows/PACo/assets/35654198/68012bbd-dfe0-4566-b534-aaf063e9ee0f)

Above, the two possible visualizations are shown:
- Elevation (#1)
- Line (#2)

When a PACo canvas component has a custom property called "cmp_Visualization", it must have one of these two values.

You can use the canvas app "PACo Examples" to experiment with, and thus better understand, this PACo canvas component.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Theme | Data | Input | Record | The theme. | See the documentation on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documentation about cmp_Visualization below. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Visualization
With visualization, the visualization of the border is meant.

There are two possible visualizations:
- Elevation
- Line

A line visualization has a border thickness of 1.

Not all PACo canvas components have a visualization option.

When a PACo canvas component has a custom property called "cmp_Visualization", it also has a custom property called "cmp_VisualizationColor". This allows a maker to set a custom border color. The default color is the color defined in the pallette slot "themePrimary".
