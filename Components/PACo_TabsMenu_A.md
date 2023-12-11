# PACo_TabsMenu_A

This page is related to version: 3.0

![image](https://github.com/formsandflows/PACo/assets/35654198/2f72dddb-c030-42cd-b78e-2d1a1779b0dd)

The selected tab in the tabs menu has a marker before the text. This is not shown in the image above because there the selected tab is "Form".

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Menu | Data | Input | Table | The tabs menu items. | See the documention about cmp_Menu below. |
| cmp_OnSelect | Event | | Boolean | When a tabs menu item is clicked on. | See the documention about cmp_OnSelect below. |
| cmp_SelectedTab | Data | Input | Number | The ID of the selected tab. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Menu
A tabs menu item has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID (number) of the tabs menu item. |
| Text | The text. |

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_TabID" which contains the ID of the tabs menu item clicked on.

### cmp_TextStyling
This custom property is of data type "Record" and has the following properties:

| Property | Description |
| :--- | :--- |
| Color | The color. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| TextBlockHeight | The height of the text block. |
