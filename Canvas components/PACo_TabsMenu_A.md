# PACo_TabsMenu_A

> [!WARNING]
> This page is a pre-release page. It contains documentation for a future release. Please look in de folder "Archive" for documentation on released versions.

This documentation page is related to version: 3.2.0

Related video page: https://www.formsandflows.nl/paco/videos/paco_tabsmenu_a/

![image](https://github.com/formsandflows/PACo/assets/35654198/2f72dddb-c030-42cd-b78e-2d1a1779b0dd)

The selected tab in the tabs menu has a bar before the text. This is not shown in the image above because there the selected tab is: Form

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Authorization | Data | Input | Table | The authorization. | See the documention about cmp_Authorization below. |
| cmp_BackgroundColor | Data | Input | Text | The color of the background. | |
| cmp_DividerColor | Data | Input | Text | The color of the divider. | |
| cmp_Menu | Data | Input | Table | The tabs menu items. | See the documention about cmp_Menu below. |
| cmp_OnSelect | Event | | None | The event fired when a tabs menu item is clicked on. | See the documention about cmp_OnSelect below. |
| cmp_SelectedColor | Data | Input | Text | The color of the bar of the selected tabs menu item (tab). | |
| cmp_SelectedTab | Data | Input | Number | The ID of the selected tabs menu item (tab). | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Authorization
An authorization item has the following properties:

| Property | Description |
| :--- | :--- |
| ID | The ID of the related tab menu item (tab). |
| Authorization | The authorization. Possible value are: Show, Hide, Disable |

The table must contain 8 items.

The same authorization setup used for the related tabs canvas component must also be used for the tabs menu canvas component.

### cmp_Menu
A tabs menu item has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID (number) of the tabs menu item. |
| Text | The text. |

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_TabID" which contains the ID of the tabs menu item clicked on.

### cmp_TextStyling
This custom property has the following properties:

| Property | Description |
| :--- | :--- |
| Color | The color. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| TextBlockHeight | The height of the text block. |
