# PACo_CommandBarMenu_A

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://user-images.githubusercontent.com/35654198/235977451-6a35b6da-012f-48ba-bbd5-719c261c28c3.png)

You can use the canvas app "PACo Examples" for a better understanding of, and to experiment with, this canvas component.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Menu | Data | Input | Table | The command bar menu items. | See the documention on cmp_Menu below. |
| cmp_OnSelect | Event | | Boolean | When a command bar menu item is clicked on. | See the documention on cmp_OnSelect below. |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention on cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of canvas component cmp_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Menu
A command bar menu item has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID (number) of the command bar menu item. |
| Image| A svg definition for the image. |
| ImagePadding | The padding of the image. |
| Text | The text. |

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_CommandID" which contains the ID of the command bar menu item clicked on.

### cmp_TextStyling
This custom property is of data type "Record" and has the following properties:

| Property | Description |
| :--- | :--- |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| TextBlockHeight | The height of the text block. |
