# PACo_Dialog_A

This canvas component is meant to be used for a dialog.

![image](https://user-images.githubusercontent.com/35654198/197049801-26e700d7-70c2-4742-b8f2-993083c4ab5c.png)

When using variables for the input properties, one dialog component can be used for multiple situations. This is implemented in the companion canvas app [PACoCo](./../PACoCo.md).

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Buttons | Table | This property determines which buttons to show. | *See the documention on buttons below.* |
| cmp_Message | Text | This property contains the body text of the dialog. | The data will be reloaded. |
| cmp_Percentage | Number | This property contains the percentage of the "border". | 20 |
| cmp_Theme | Record | This property contains the theme to use for the dialog. | *See the documention on theming.* |
| cmp_Transparency| Number | This property contains the "border" transparency. It must be a value between 0 and 1. | 0.2 |
| cmp_Title | Text | This property contains the title of the dialog. | Reload |
| cmp_Visualization | Text | This property contains the visualization. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | This property contains the color to use in the visualization. | #0078d4 |

### Buttons
A dialog can show 1 or 2 buttons depending on its need. If only one button is needed, only one table item must be added. One button will have a centered alignment. Two buttons will have a right alignment.

A button has the following properties:

| Property | Description |
| :--- | :--- |
| Text | The text to display in the button. |
| Title | The internal name of the button. This is needed to support multilingual canvas apps. |
| Type | Possible values: Primary or secondary. |
| Width | The width of the button. |

The example below is used in the screenshot shown above.

`Table({Text:"Ok", Title:"Ok", Type:"Primary", Width:160}, {Text:"Cancel", Title:"Cancel", Type:"Secondary", Width:160})`

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the property "OnSelect" of the buttons. It contains a required parameter (cmp_Param_Button) which contains the title of the button clicked on. |
