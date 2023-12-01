# PACo_Tile_A

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://user-images.githubusercontent.com/35654198/235983122-1b9fdc5d-9686-4859-82de-d9c967dcd95b.png)

You can use the canvas app "PACo Examples" for a better understanding of, and to experiment with, this canvas component.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Text | Data | Input | Text | The text to shown in the upper section of the tile. | |
| cmp_TextStyling | Data | Input | Table | Text properties. | See the documention on cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Value | Data | Input | Number | The value to show in the lower section of the tile. | |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of canvas component cmp_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_TextStyling
This custom property is of data type "Table" and a record has the following properties:

| Property | Description |
| :--- | :--- |
| Align | The horizontal alignment. |
| ID | An unique ID for the section (Text or Value). |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| VerticalAlign | The vertical alignment. |
