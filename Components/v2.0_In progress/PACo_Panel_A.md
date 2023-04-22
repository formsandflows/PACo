# PACo_Panel_A

This canvas component is meant to be used for a panel.

![PACo_Panel](https://user-images.githubusercontent.com/35654198/197223171-3e9f5821-5623-4991-9a1c-169d4cc5bc3b.png)

A panel is shown when an item in the details list component is clicked on (This must be configured in the details list component!). With a panel, addition item properties can be shown than is shown in the details list component. A vertical scrollbar appears when there is more data to show than fits on the screen.

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Buttons | Table | This property contains the buttons to show on the bottom of the panel. | *See the documention on panel buttons below.* |
| cmp_Commands | Record | This property contains the panel command items to show in the top of the panel. | *See the documention on panel commands below.* |
| cmp_Record | Table | This property contains the data to show in the panel. | *See the documention on panel data below.* |
| cmp_Theme | Record | This property contains the theme to use for the panel. | *See the documention on theming.* |
| cmp_Visualization | Text | This property contains the visualization. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | This property contains the color to use in the visualization. | #0078d4 |
| cmp_Width | Number | This property contains the width of the panel. | 400 |

### Panel buttons

The setup of the related property is such that more buttons can be shown but only one button is supported (read: configured/tested)!

The panel button has the following properties:

| Property | Description |
| :--- | :--- |
| Text | The text to display in the button. |
| Title | The internal name of the button. This is needed to support multilingual canvas apps. |
| Type | Possible values: Primary or secondary. |
| Width | The width of the button. |

The example below is used in the screenshot shown above.

`Table({Text:"Ok", Title:"Ok", Type:"Primary", Width:160})`

### Panel command items
A panel command item has the following properties:

| Property | Description |
| :--- | :--- |
| Icon | The icon to show. |
| Text | The text to display in the related label control. |
| Title | The internal name of the panel command item. This is needed to support multilingual canvas apps. |
| Width | The width of the related label control. |

A maximum of 2 commands are supported (read: configured/tested)!

Example:

`{Command1: {Icon:Icon.Edit, Text:"Edit", Title:"Edit", Width:48}, Command2: {Icon:Icon.Trash, Text:"Delete", Title:"Delete", Width:64}}`

Setting the width to 0 makes sure that the related panel command item is not shown.

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

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnCommandSelect | This property is related to the property "OnSelect" of all panel command items. It contains a required parameter (cmp_Param_Command) which contains the title of the command item clicked on. |
| cmp_OnSelect | This property is related to the property "OnSelect" of the panel button. |
