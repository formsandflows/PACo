This canvas component is meant to be used for a command bar.

![PACo_CommandBar](https://user-images.githubusercontent.com/35654198/197222781-1416d2e2-b950-4623-a125-fe4e526c3211.png)

## **Input properties**

| Property | Type | Description | Example |
| - | - | - | - |
| cmp_Commands | Record | This property contains the command bar items. | *See the documention on command bar items below.* |
| cmp_ElevationColor | Text | This property contains the color to use in the elevation of the command bar. | #0078d4 |
| cmp_SelectedItems | Text | This property contains an indicator if 0, 1 or more than 1 items are selected in the details list component. | *See the documention on selected items below.* |
| cmp_Theme | Record | This property contains the theme to use for the command bar. | *See the documention on themes.* |

### Command bar items
Because the command bar items will have a different width, using a gallary for it was not possible. A record was used instead. 
There is also a maximum of 8 command bar items (though you can add more yourself).

A command bar item has the following properties:

| Property | Description |
| - | - |
| Icon | The icon to use. |
| SelectedItems | When to show the command bar item. *See the documention on selected items below.* |
| Title | The title of the related label control. |
| Width | The width of the related label control. |

Example:
{Icon1:Icon.Add, Title1:"New", Width1:50, SelectedItems1:"#0#", Icon2: Icon.Edit, Title2:"Edit", Width2:48, SelectedItems2:"#1#", ...}

### Selected items
A command bar item can be shown when there are 0, 1 and more than 1 items are selected in the details list component.

To make this possible, a fixed setup must be followed for the property "SelectedItems". This propery must contain a fixed string depending on when to show the command bar item.

- #0# > The command bar item is shown when no items are selected.
- #1# > The command bar item is shown when 1 item is selected.
- #2# > The command bar item is shown when more than 1 item is selected.

Example:
A command bar item which has "#1#2#" set for the "SelectedItems" is only shown when 1 or more than 1 item is selected in the details list component.

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| - | - |
| cmp_OnSelect | This property is related to the OnSelect property of all icons. It contains a required parameter (cmp_Param_Command) which contains the title of the command clicked on. |
