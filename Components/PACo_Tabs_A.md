# PACo_Tabs_A

This page is related to version: 3.0

![image](https://github.com/formsandflows/PACo/assets/35654198/2a2b1389-0718-4400-b853-c810ae116892)

This PACo canvas component is responsive.

A menu indicator (3 dots) is shown when there are tabs to show which cannot be shown because the width is to small. The idea is that when the menu indicator is clicked on, a tabs menu is shown. This tabs is another PACo canvas component: PACo_TabsMenu_A

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_SelectedTab | Data | Input | Number | The ID of the selected tab. | |
| cmp_LastTab | Data | Output | Number | The last tab still visible. | |
| cmp_OnSelect | Event | | Boolean | When a tab is clicked on. | See the documention about cmp_OnSelect below. |
| cmp_Tabs | Data | Input | Record | The tabs. | See the documention about cmp_Tabs below. |
| cmp_TabSpacing | Data | Input | Number | The space between tabs. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Tabs
A tab has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID (number) of the tab. |
| Text | The text. |

This component allows for up to 8 possible command bar items.

When a command bar item shoud not be used:
- set the property "SelectedItems" to "##"

, for the related command bar item. This property can thus be used for logic when to show the related command bar item. Example: Because of RBAC (Role Based Access Control).

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_CommandID" which contains the ID of the command bar item clicked on. When the menu indicator is clicked on, a 0 (zero) is returned.

### cmp_SelectedItems
A command bar item can be shown for the situations when 0, 1 or more than 1 items are selected in the related details list canvas component. There are 3 details list canvas components (PACo_DetailsList_A, PACo_DetailsList_B, PACo_DetailsList_C) part of PACo.

To make this possible, a fixed setup must be followed for the property "SelectedItems" of a command bar item and for the custom property "cmp_Selecteditems" of the canvas component.

#### Property "SelectedItems" of a command bar item
This property is used to determine when the command bar item must be shown.

- #0# > The command bar item is shown when no items are selected in the details list.
- #1# > The command bar item is shown when 1 item is selected in the details list.
- #2# > The command bar item is shown when more than 1 item is selected in the details list.

Above are example of single situations. The property "SelectedItems" of a command bar item can also be used for multiple situations. Example: A command bar item which has "#0#1#2#" set for its property "SelectedItems" is shown for the situations when 0, 1 or more than 1 item is selected in the details list.

#### Custom property "cmp_SelectedItems" of the component
This property determines if 0, 1 or more than 1 items are selected in the details list.

- #0# > Command bar items with "#0#" in their property "SelectedItems" are shown.
- #1# > Command bar items with "#1#" in their property "SelectedItems" are shown.
- #2# > Command bar items with "#2#" in their property "SelectedItems" are shown.

### cmp_TextStyling
This custom property is of data type "Record" and has the following properties:

| Property | Description |
| :--- | :--- |
| Color | The color. |
| Font | The font. |
| FontSize | The font size. |
