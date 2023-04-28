# PACo_CommandBar_B

This canvas component is meant to be used for a command bar.

[[ IMAGE ]]

A command bar item consists of 4 controls:
* An image control to show the icon.
* A html control to determine the width of the label control.
* A label control to show the text.
* A transparent icon which is used as an overlay. It spans the whole command bar item and its OnSelect property is related to the behavior property "cmp_OnSelect".

This is a responsive component. A menu indicator (3 dots) is shown when there are command bar items to show but which cannot because the width of the command bar is to small. When the menu indicator is clicked on, a command bar menu is shown. This command bar menu is another canvas component (PACo_CommandBarMenu) which is also part of PACo-Core.

The menu indicator conists of 2 controls:
* A label control containing the 3 dots.
* A transparent icon which is used as an overlay. It spans the whole menu indicator and its OnSelect property is related to the behavior property "cmp_OnSelect".

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Commands | Record | The command bar items. | *See the documention on command bar items below.* |
| cmp_ImagePadding | Number | The padding of the icons. | 10 |
| cmp_SelectedItems | Text | Indicator number of selected items (0, 1 or more than 1) in the details list component. | *See the documention on selected items below.* |
| cmp_Theme | Record | The theme to use. | *See the documention on theming.* |
| cmp_Visualization | Text | The visualization to use. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | The color of the visualization. | #0078d4 |

### Command bar items
A command bar item has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID (number) of the command bar item. |
| Image | A svg definition to be used as an icon. |
| SelectedItems | When to show the command bar item. *See the documention on selected items below.* |
| Text | The text to display in the related label control. |
| Title | The internal name of the command bar item. This is needed to support multilingual canvas apps. |

This component allows for up to 8 possible command bar items.

When a command bar item shoud not be used:

- set the property "SelectedItems" to "##".
- set the property "Text" to an empty string ("").
- set the property "Title" to an empty string ("").

, for the related command bar item.

### Selected items
A command bar item can be shown for the situations when 0, 1 or more than 1 items are selected in the details list component which is also part of PACo-Core.

To make this possible, a fixed setup must be followed for the property "SelectedItems" of a command bar item and of the property "cmp_Selecteditems" of the component.

#### Property "SelectedItems" of a command bar item

This property is used to determine when the command bar item must be shown.

- #0# > The command bar item is shown when no items are selected in the details list component.
- #1# > The command bar item is shown when 1 item is selected in the details list component.
- #2# > The command bar item is shown when more than 1 item is selected in the details list component.

Above are example of single situations. The property "SelectedItems" of a command bar item can also be used for multiple situations. Example: A command bar item which has "#0#1#2#" set for its property "SelectedItems" is shown for the situations when 0, 1 or more than 1 item is selected in the details list component which is also part of PACo-Core.

#### Property "cmp_SelectedItems" of the component

This property determines if 0, 1 or more than 1 items are selected in the details list component.

- #0# > Command bar items with "#0#" in their property "SelectedItems" are shown.
- #1# > Command bar items with "#1#" in their property "SelectedItems" are shown.
- #2# > Command bar items with "#2#" in their property "SelectedItems" are shown.

## **Output properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_MenuPropertyX | Number | The X value for the command bar menu.  | 720 |
| cmp_LastCommand | Number | The last command bar item still visible. | 5 |

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the property "OnSelect" of several icon controls. It contains a required parameter (cmp_Param_Command) which contains the property "Title" of the command bar item clicked on. |
