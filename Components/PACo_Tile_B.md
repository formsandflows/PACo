# PACo_Tile_B

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://github.com/formsandflows/PACo/assets/35654198/029ccce4-b9bc-4a6b-9c49-8400549929ac)

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Clickable | Data | Input | Boolean | If the tile is clickable or not. | |
| cmp_OnSelect | Event | | Boolean | When the tile is clicked on and is clickable. |
| cmp_Text | Data | Input | Text | The text. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_TextStyling
This custom property is of data type "Record" and has the following properties:

| Property | Description |
| :--- | :--- |
| Align | The horizontal alignment. |
| Color | The color. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| Padding | The padding. |
| VerticalAlign | The vertical alignment. |
