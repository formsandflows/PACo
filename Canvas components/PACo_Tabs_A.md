# PACo_Tabs_A

This documentation page is related to version: 3.3.0

Related video page: https://www.formsandflows.nl/paco/videos/paco_tabs_a/

![image](https://github.com/formsandflows/PACo/assets/35654198/2a2b1389-0718-4400-b853-c810ae116892)

A menu indicator (3 dots) is shown at the right when there are tabs to show which cannot be shown because the width is too small. The idea is that when the menu indicator is clicked on, a tabs menu is shown. This tabs menu also shown in the image above and is another PACo canvas component: PACo_TabsMenu_A

The selected tab has a bar below the text. In the image above, the selected tab is: Form

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_BackgroundColor | Data | Input | Text | The color of the background. | This is a required property. If no background color is given, tabs which are disabled will not be alighned properly. |
| cmp_LastTab | Data | Output | Number | The last tab still visible. | |
| cmp_OnSelect | Event | | None | The event fired when a tab is clicked on. | See the documention about cmp_OnSelect below. |
| cmp_SelectedColor | Data | Input | Text | The color of the bar of the selected tab. | |
| cmp_SelectedTab | Data | Input | Number | The ID of the selected tab. | |
| cmp_Tabs | Data | Input | Record | The tabs. | See the documention about cmp_Tabs below. |
| cmp_TabSpacing | Data | Input | Number | The space between tabs. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_TabID" which contains the ID of the tab clicked on. When the menu indicator is clicked on, a 0 (zero) is returned.

### cmp_Tabs
A tab has the following properties:

| Property | Description |
| :--- | :--- |
| Disabled | If the tab is disabled or not. |
| Hidden | If the tab is hidden or not. |
| ID | An unique ID (number) of the tab. |
| Text | The text. |

This canvas component allows for up to 8 possible tabs. When a tab shoud not be used, its property "Text" should be empty.

### cmp_TextStyling
This custom property has the following properties:

| Property | Description |
| :--- | :--- |
| Color | The color. |
| Font | The font. |
| FontSize | The font size. |
