# cmp_Panel_A

This canvas component is meant to be used for a panel.

![PACo_Panel](https://user-images.githubusercontent.com/35654198/197223171-3e9f5821-5623-4991-9a1c-169d4cc5bc3b.png)

A panel is shown when an item in the details list component is clicked on (This must be configured in the details list component!). More data can be shown than is shown in the details list component. A vertical scrollbar appear when there is more data to shown on the screeen.

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Buttons | Table | This property contains the buttons to show on the bottom of the panel. | *See the documention on panel buttons below.* |
| cmp_Commands | Record | This property contains the command to show in the top of the panel. | *See the documention on panel commands below.* |
| cmp_Record | Table | This property contains the data to show in the panel. | *See the documention on panel data below.* |
| cmp_Theme | Record | This property contains the theme to use for the panel. | *See the documention on theming.* |
| cmp_Visualization | Text | This property contains the visualization. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | This property contains the color to use in the visualization. | #0078d4 |
| cmp_Width | Number | This property contains the width of the panel. | 400 |

### Panel buttons

The setup of the related property is such that more buttons can be shown. Only one button is supported (read: configured/tested)! A button can be configured with a title and a type (Primary or secondary).

Example:

`Table({Title:"Ok", Type:"Primary"})`

### Panel data
A gallery is used to show data in the panel. A gallery item has the following properties:

| Property | Description |
| :--- | :--- |
| Label | The label text. |
| LabelHeight | The height of the label. |
| Text | The gallery item text. |
| TextHeight | The height of the gallery item. |

The LabelHeight and TextHeight properties are not required. A value of 40 is used in case the properties are not defined.

Example:

`Table({Label:"Label 1", Text:"Hello world!"}, {Label:"Label 2", Text:"Hello world!", TextHeight: 120})`

### Panel commands
A panel command item has the following properties:

| Property | Description |
| :--- | :--- |
| Icon | The icon to use. |
| Title | The title of the related label control. |
| Width | The width of the related label control. |

A maximum of 2 commands are supported (read: configured/tested)!

Example:

`{Icon1:Icon.Edit, Title1:"Edit", Width1:48, Icon2:Icon.Trash, Title1:"Delete", Width1:64}`

Setting the width to 0 makes sure that the related command is not shown.

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnCommandSelect | This property is related to the property "OnSelect" of all panel commands. It contains a required parameter (cmp_Param_Command) which contains the title of the command clicked on. |
| cmp_OnSelect | This property is related to the property "OnSelect" of all panel buttons. |
