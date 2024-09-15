# PACo_CommandBarMenu_A

>  [!WARNING]
> This is page contains pre-release information is can be not up-to-date yet. The documention of the latest version is in the archive folder.

This documentation page is related to version: 3.3.0

Related video page: https://www.formsandflows.nl/paco/videos/paco_commandbarmenu_a/

![image](https://github.com/formsandflows/PACo/assets/35654198/45b79e8c-b3c2-47bf-883d-1e5f8d0546cc)

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_BackgroundColor | Data | Input | Text | The color of the background. | |
| cmp_DividerColor | Data | Input | Text | The color of the divider. | |
| cmp_Menu | Data | Input | Table | The command bar menu items (commands). | See the documention about cmp_Menu below. |
| cmp_OnSelect | Event | | None | The event fired when a command bar menu item (command) is clicked on. | See the documention about cmp_OnSelect below. |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Menu
An command bar menu item (command) has the following properties:

| Property | Description |
| :--- | :--- |
| Disabled | If the command bar menu item is disabled or not. |
| Hidden | If the command bar menu item is hidden or not. |
| ID | An unique ID (number) of the command bar menu item (command). |
| Image | A svg definition for the image. |
| ImageHeight | The height and width of the image. |
| ImagePadding | The padding of the image. |
| SelectedItems | When to show the command bar menu item (command). See the documention of PACo canvas component PACo_CommandBar_B. |
| Text | The text. |

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_CommandID" which contains the ID of the command bar menu item (command) clicked on.

### cmp_TextStyling
This custom property has the following properties:

| Property | Description |
| :--- | :--- |
| Color | The color. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| Padding | The padding of the text. |
