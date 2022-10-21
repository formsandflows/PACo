This canvas component is meant to be used for a panel.

![PACo_Panel](https://user-images.githubusercontent.com/35654198/197223171-3e9f5821-5623-4991-9a1c-169d4cc5bc3b.png)

## **Input properties**

| Property | Type | Description | Example |
| - | - | - | - |
| cmp_Buttons | Table | This property contains the buttons to show on the bottom of the panel. | *See the documention on panel buttons below.* |
| cmp_Commands | Record | This property contains the command to show in the top of the panel. | *See the documention on panel commands below.* |
| cmp_ElevationColor | Text | This property contains the color to use in the elevation of the panel. | #0078d4 |
| cmp_Record | Table | This property contains the data to show in the panel. | *See the documention on panel data below.* |
| cmp_Theme | Record | This property contains the theme to use for the panel. | *See the documention on themes.* |
| cmp_Width | Number | This property contains the width of the panel. | 400 |

### Panel buttons

The setup of the related property is such that more buttons can be shown. Only one button is supported (read: configured/tested)!

Example:

Table({Title:"Ok", Type:"Primary"})

### Panel data

A gallery is used to show data in the panel.

Example:

Table({Label:"Label 1", Text:"Hello world!"}, {Label:"Label 2", Text:"Hello world!"})

### Panel commands

Only a maximum of 2 commands is supported (read: configured/tested)!

Example:

{Icon1:Icon.Edit, Title1:"Edit", Width1:48, Icon2:Icon.Trash, Title1:"Delete", Width1:64}

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| - | - |
| cmp_OnCommandSelect | This property is related to the OnSelect property of all panel commands. It contains a required parameter (cmp_Param_Command) which contains the title of the command clicked on. |
| cmp_OnSelect | This property is related to the OnSelect property of all panel buttons. |
