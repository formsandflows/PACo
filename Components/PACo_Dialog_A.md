# PACo_Dialog_A

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://user-images.githubusercontent.com/35654198/235979899-d2168297-2283-498b-8148-0c03e1828836.png)

This is a responsive canvas component.

When using variables for the input properties, one dialog component can be used for multiple situations. This is implemented in the companion canvas app [PACoCo](./../PACoCo.md).

The width of a button depends on a minimal width property, if an icon is added and the length of the text to show.

You can use the canvas app "PACo Examples" for a better understanding of, and to experiment with, this canvas component.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Buttons | Data | Input | Table | The buttons to show. | See the documention on cmp_Buttons below. |
| cmp_Message | Data | Input | Text | The message of the dialog. | |
| cmp_OnSelect | Event | | Boolean | When a button is clicked on. | |
| cmp_Percentage | Data | Input | Number | The percentage of the total width for the "border". | |
| cmp_TextStyling | Data | Input | Table | Text properties. | See the documention on cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Title | Data | Input | Text | The title of the dialog. | |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of component cmp_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Buttons
A dialog can show 0, 1 or 2 buttons depending on its need. A button can contain an icon (image). If only one button is needed, only one table item must be added. One button will have a centered alignment. Two buttons will have a right alignment. If 0 buttons should be shown, only one table item must be added where the properties "Text" and "Title" should be empty.

A button has the following properties:

| Property | Description |
| :--- | :--- |
| Image | A svg definition for an image. |
| ImagePadding | The padding of the image. |
| MinimalWidth | The minimal width of the button. |
| Text | The text to display in the button. |
| Title | The internal name of the button. This is needed to support multilingual canvas apps. |
| Type | Possible values: Primary, Secondary. |

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_Button" which contains the title of the button clicked on.

### cmp_TextStyling
This custom property is of data type "Table" and a record has the following properties:

| Property | Description |
| :--- | :--- |
| Align | The text alignment. |
| ButtonHeight | The button height. |
| ID | An unique ID for the title/message. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |

Not all properties are used by all controls.
