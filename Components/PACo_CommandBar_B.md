# PACo_CommandBar_B

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://user-images.githubusercontent.com/35654198/235978488-10113e29-f5ff-4fd5-8254-ac7ae55d49d8.png)

This is a responsive canvas component. A menu indicator (3 dots) is shown when there are command bar items to show which cannot be shown because the width of the command bar is to small. When the menu indicator is clicked on, a command bar menu is shown. This command bar menu is another canvas component (PACo_CommandBarMenu_A) which is also part of PACo.

This canvas component has its "OnReset" property configured. When a canvas component instance is reset, the text shown in the command bar items is reset.

You can use the canvas app "PACo Examples" for a better understanding of, and to experiment with, this canvas component.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Commands | Data | Input | Record | The command bar items. | See the documention on cmp_Commands below. |
| cmp_LastCommand | Data | Output | Number | The last command bar item still visible. | |
| cmp_MenuPropertyX | Data | Output | Number | The X value for the command bar menu.  | |
| cmp_OnSelect | Event | | Boolean | When a command bar item is clicked on. | See the documention on cmp_OnSelect below. |
| cmp_SelectedItems | Data | Input | Text | Indicator of the number of selected items (0, 1 or more than 1) in the related details list. | See the documention on cmp_SelectedItems below. |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention on cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Commands
A command bar item has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID (number) of the command bar item. |
| Image | A svg definition for the image. |
| ImagePadding | The padding of the image. |
| SelectedItems | When to show the command bar item. See the documention on cmp_SelectedItems below. |
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
