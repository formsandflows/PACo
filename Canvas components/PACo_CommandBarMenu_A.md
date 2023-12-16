# PACo_CommandBarMenu_A

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://github.com/formsandflows/PACo/assets/35654198/45b79e8c-b3c2-47bf-883d-1e5f8d0546cc)

This PACo canvas component is responsive.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Menu | Data | Input | Table | The command bar menu items (commands). | See the documention about cmp_Menu below. |
| cmp_OnSelect | Event | | Boolean | When a command bar menu item (command) is clicked on. | See the documention about cmp_OnSelect below. |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Menu
A command bar menu item (command) has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID (number) of the command bar menu item (command). |
| Image| A svg definition for the image. |
| ImagePadding | The padding of the image. |
| SelectedItems | When to show the command bar menu item (command). See the documention of PACo canvas component PACo_CommandBar_B. |
| Text | The text. |

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_CommandID" which contains the ID of the command bar menu item (command) clicked on.

### cmp_TextStyling
This custom property is of data type "Record" and has the following properties:

| Property | Description |
| :--- | :--- |
| Color | The color. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| TextBlockHeight | The height of the text block. |
