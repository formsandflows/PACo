# PACo_Dialog_A

This canvas component is meant to be used for a dialog.

[[ IMAGE ]]

When using variables for the input properties, one dialog component can be used for multiple situations. This is implemented in the companion canvas app [PACoCo](./../PACoCo.md).

The width of a button depends on a minimal width property, if an icon is added and the length of the text to show.

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Buttons | Table | The buttons to show. | *See the documention on buttons below.* |
| cmp_Message | Text | The message of the dialog. | The data will be reloaded. |
| cmp_Percentage | Number | The percentage of the total width for the "border". | 20 |
| cmp_Theme | Record | The theme to use. | *See the documention on theming.* |
| cmp_Title | Text | The title of the dialog. | Reload |
| cmp_Visualization | Text | The visualization to use. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | The color of the visualization. | #0078d4 |

### Buttons
A dialog can show 0, 1 or 2 buttons depending on its need. A button can contain an icon (image). If only one button is needed, only one table item must be added. One button will have a centered alignment. Two buttons will have a right alignment. If 0 buttons should be shown, only one table item must be added where the properties "Text" and "Title" should be empty.

A button has the following properties:

| Property | Description |
| :--- | :--- |
| Image | A svg definition to be used as an icon. |
| ImagePadding | The padding of the icon. |
| MinimalWidth | The minimal width of the button. |
| Text | The text to display in the button. |
| Title | The internal name of the button. This is needed to support multilingual canvas apps. |
| Type | Possible values: Primary, Secondary. |

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the property "OnSelect" of the button(s). It contains a required parameter (cmp_Param_Button) which contains the title of the button clicked on. |
