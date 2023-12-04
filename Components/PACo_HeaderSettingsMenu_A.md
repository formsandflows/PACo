# PACo_HeaderSettingsMenu_A

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://user-images.githubusercontent.com/35654198/235982163-5c2ef64a-9f0f-4e69-8c3a-5003116f13f3.png)

This is a responsive canvas component.

You can use the canvas app "PACo Examples" for a better understanding of, and to experiment with, this canvas component.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Menu | Data | Input | Table | The settings menu items. | See the documention on cmp_Menu below. |
| cmp_OnSelect | Event | | Boolean | When a settings menu item is clicked on. | See the documention on cmp_OnSelect below. |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention on cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |
| cmp_Width | Data | Input | Number | The width of the settings menu. | |

### cmp_Menu
A settings menu item has the following properties:

| Property | Description |
| :--- | :--- |
| Disabled | If the menu item is disabled or not. |
| ID | The unique ID (number) of the settings menu item used in the custom property "cmp_OnSelect". |
| Order | The order of the settings menu item. |
| Screen | The screen control to navigate to. |
| Text | The text. |

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_SettingID" which contains the ID of the settings menu item clicked on.

### cmp_TextStyling
This custom property is of data type "Record" and has the following properties:

| Property | Description |
| :--- | :--- |
| Align | The horizontal alignment. |
| Color | The color. |
| ColorDisabled | The color when the settings menu item is disabled. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| Padding | The padding. |
| TextBlockHeight | The height of the text block. |
| VerticalAlign | The vertical alignment. |