# PACo_CommandBarMenu_A

> [!CAUTION]
> This documentation page is currently in the process of being upgraded to canvas component version 3.1.0 which will be released very soon.

This documentation page is related to version: 3.1.0

Related video page: https://www.formsandflows.nl/paco/videos/paco_commandbarmenu_a/

![image](https://github.com/formsandflows/PACo/assets/35654198/45b79e8c-b3c2-47bf-883d-1e5f8d0546cc)

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Authorization | Data | Input | Table | The authorization table. | See the documention about cmp_Authorization below. |
| cmp_Menu | Data | Input | Table | The command bar menu items (commands). | See the documention about cmp_Menu below. |
| cmp_OnSelect | Event | | Boolean | When a command bar menu item (command) is clicked on. | See the documention about cmp_OnSelect below. |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Authorization
An authorization item has the following properties:

| Property | Description |
| :--- | :--- |
| ID | The ID of the releated command bar menu item (command). |
| Authorization | The authorization. See the documention of PACo canvas component PACo_CommandBar_B. |

The table must contain 8 items.

### cmp_Menu
A command bar menu item (command) has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID (number) of the command bar menu item (command). |
| Image | A svg definition for the image. |
| ImagePadding | The padding of the image. |
| SelectedItems | When to show the command bar menu item (command). See the documention of PACo canvas component PACo_CommandBar_B. |
| Text | The text. |

The table must contain 8 items.

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
