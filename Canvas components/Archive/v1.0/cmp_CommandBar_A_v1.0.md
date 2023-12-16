# cmp_CommandBar_A

This canvas component is meant to be used for a command bar.

![PACo_CommandBar](https://user-images.githubusercontent.com/35654198/197222781-1416d2e2-b950-4623-a125-fe4e526c3211.png)

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Commands | Record | This property contains the command bar items. | *See the documention on command bar items below.* |
| cmp_ElevationColor | Text | This property contains the color to use in the elevation of the command bar. | #0078d4 |
| cmp_SelectedItems | Text | This property contains an indicator if 0, 1 or more than 1 items are selected in the details list component. | *See the documention on selected items below.* |
| cmp_Theme | Record | This property contains the theme to use for the command bar. | *See the documention on theming.* |

### Command bar items
A command bar item has the following properties:

| Property | Description |
| :--- | :--- |
| Icon | The icon to use. |
| SelectedItems | When to show the command bar item. *See the documention on selected items below.* |
| Title | The title of the related label control. |
| Width | The width of the related label control. |

Example:

`{Icon1:Icon.Add, Title1:"New", Width1:50, SelectedItems1:"#0#", Icon2: Icon.Edit, Title2:"Edit", Width2:48, SelectedItems2:"#1#", ...}`

A record is used to define the command bar. Because command bar items will have a different width, using a gallery for the commands was not possible. This component contains up to 8 command slots. How many to actually use is configured in the record. When a command slot shoud not be used:

- The property "Title#" must be set to an empty string ("").
- The property "Width#" must be set to 0.
- The property "SelectedItems#" must be set to "##".

, where # is the number of the command bar item.

### Selected items
A command bar item can be shown when there are 0, 1 and more than 1 items are selected in the details list component.

To make this possible, a fixed setup must be followed for the property "SelectedItems" of a command bar item and of the property "cmp_Selecteditems" of the component.

#### Property "SelectedItems" of a command bar item

This property is used to determine when the command bar item must be shown.

- #0# > The command bar item is shown when no items are selected.
- #1# > The command bar item is shown when 1 item is selected.
- #2# > The command bar item is shown when more than 1 item is selected.

Example: A command bar item which has "#1#2#" set for its property "SelectedItems" is shown when 1 or more than 1 item is selected in the details list component.

#### Property "cmp_SelectedItems" of the component

This property determine if 0, 1 or more than 1 items are selected in the details list component.

- #0# > Command bar items with "#0#" in their property "SelectedItems" are shown.
- #1# > Command bar items with "#1#" in their property "SelectedItems" are shown.
- #2# > Command bar items with "#2#" in their property "SelectedItems" are shown.

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the property "OnSelect" of all icons. It contains a required parameter (cmp_Param_Command) which contains the title of the command clicked on. |
