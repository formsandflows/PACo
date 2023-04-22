# PACo_CommandBar_B

This canvas component is meant to be used for a command bar.

A command item consists of 4 controls:
* An image control to show the icon.
* A html control to determine the width of the label control.
* A label control to show the text.
* An icon which is used as an overlay. It spans the whole command item and its OnSelect property is related to the behavior property "cmp_OnSelect".

The menu conists of 2 controls:
* A label control containing the three dots.
* An icon which is used as an overlay. It spans the whole command item and its OnSelect property is related to the behavior property "cmp_OnSelect".

The menu is another component to show dependent on the output property "cmp_MenuPropertyVisible".

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Commands | Record | This property contains the command bar items. Every command has its own record. | *See the documention on command bar items below.* |
| cmp_SelectedItems | Text | This property contains an indicator if 0, 1 or more than 1 items are selected in the details list component. | *See the documention on selected items below.* |
| cmp_Theme | Record | This property contains the theme to use for the command bar. | *See the documention on theming.* |
| cmp_Visualization | Text | This property contains the visualization. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | This property contains the color to use in the visualization. | #0078d4 |

### Command bar items
A command bar item has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID (number) of the item. |
| Image | A svg definition to be used as an icon. |
| SelectedItems | When to show the command bar item. *See the documention on selected items below.* |
| Text | The text to display in the related label control. |
| Title | The internal name of the command bar item. This is needed to support multilingual canvas apps. |

A record is used to define the command bar. Because command bar items have different widths, using a gallery for the command bar items was not possible. This component contains up to 8 command bar item slots. How many to actually use is configured in the record. When a command bar item slot shoud not be used:

- The property "SelectedItems" must be set to "##".
- The property "Text" must be set to an empty string ("").
- The property "Title" must be set to an empty string ("").

, for the related command bar item.

### Selected items
A command bar item can be shown when there are 0, 1 and more than 1 items are selected in the details list component.

To make this possible, a fixed setup must be followed for the property "SelectedItems" of a command bar item and of the property "cmp_Selecteditems" of the component.

#### Property "SelectedItems" of a command bar item

This property is used to determine when the command bar item must be shown.

- #0# > The command bar item is shown when no items are selected.
- #1# > The command bar item is shown when 1 item is selected.
- #2# > The command bar item is shown when more than 1 item is selected.

Above are example of single situations. The property "SelectedItems" of a command bar item can also be used for multiple situations. Example: A command bar item which has "#0#1#2#" set for its property "SelectedItems" is shown when 0, 1 or more than 1 item is selected in the details list component.

#### Property "cmp_SelectedItems" of the component

This property determines if 0, 1 or more than 1 items are selected in the details list component.

- #0# > Command bar items with "#0#" in their property "SelectedItems" are shown.
- #1# > Command bar items with "#1#" in their property "SelectedItems" are shown.
- #2# > Command bar items with "#2#" in their property "SelectedItems" are shown.

## **Output properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_MenuPropertyX | Number | This property contains the X value for the menu.  | 720 |
| cmp_MenuPropertyVisible | Boolean | This property determines if the menu should be shown or not. | true |
| cmp_LastCommand | Number | This property contains the property last that command bar item that is still visible. | 5 |

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the property "OnSelect" of several icon controls. It contains a required parameter (cmp_Param_Command) which contains the property "Title" of the command clicked on. |
