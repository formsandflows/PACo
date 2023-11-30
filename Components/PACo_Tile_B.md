# PACo_Tile_B

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://user-images.githubusercontent.com/35654198/235983204-0bf827c7-0985-47b4-ab34-31d5e8166edd.png)

You can use the canvas app "PACo Examples" for a better understanding of, and to experiment with, this canvas component.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Clickable | Data | Input | Boolean | If the tile is clickable or not. | |
| cmp_OnSelect | Event | | Boolean | When the tile is clicked on and is clickable. |
| cmp_Text | Data | Input | Text | The text. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention on cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of canvas component cmp_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_TextStyling
This custom property is of data type "Record" and has the following properties:

| Property | Description |
| :--- | :--- |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
