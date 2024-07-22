# PACo_HeaderSettingsMenu_A

> [!WARNING]
> This page is a pre-release page. It contains documentation for a future release. Please look in de folder "Archive" for documentation on released versions.

This documentation page is related to version: 3.2.0

Related video page: https://www.formsandflows.nl/paco/videos/paco_headersettingsmenu_a/

![image](https://github.com/formsandflows/PACo/assets/35654198/e780d19a-5b4d-4b39-acb5-06fc42aacde2)

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_BackgroundColor | Data | Input | Text | The color of the background. | |
| cmp_DividerColor | Data | Input | Text | The color of the divider. | |
| cmp_Menu | Data | Input | Table | The settings menu items. | See the documention about cmp_Menu below. |
| cmp_OnSelect | Event | | None | The event fired when a settings menu item is clicked on. | See the documention about cmp_OnSelect below. |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |
| cmp_Width | Data | Input | Number | The width of the settings menu. | |

### cmp_Menu
A settings menu item has the following properties:

| Property | Description |
| :--- | :--- |
| Disabled | If the menu item is disabled or not. |
| ID | An unique ID (number) of the settings menu item used in the custom property "cmp_OnSelect". |
| Order | The order of the settings menu item. |
| Screen | The screen to navigate to. |
| Text | The text. |

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_SettingID" which contains the ID of the settings menu item clicked on.

### cmp_TextStyling
This custom property has the following properties:

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
