# PACo_Dialog_A

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://github.com/formsandflows/PACo/assets/35654198/ad42c67b-c4c2-4068-ad4d-2b3f88f36088)

This PACo canvas component is responsive.

When using variables for the input properties, one dialog component can be used for multiple situations. This is implemented in the canvas app [PACoCo](https://www.formsandflows.nl/paco/pacoco/).

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Buttons | Data | Input | Table | The buttons to show. | See the documention about cmp_Buttons below. |
| cmp_Message | Data | Input | Text | The message of the dialog in plain text. | |
| cmp_MessageHTML | Data | Input | Text | The message of the dialog in HTML. | |
| cmp_OnSelect | Event | | Boolean | When a button is clicked on. | |
| cmp_Percentage | Data | Input | Number | The percentage of the total width for the "border". | |
| cmp_TextStyling | Data | Input | Table | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Title | Data | Input | Text | The title of the dialog. | |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

When both plain text (cmp_Message) and HTML (cmp_MessageHTML) are provided for the message, HTML is shown.

The title of the dialog is not shown when the custom property "cmp_Title" contains no text.

### cmp_Buttons
A dialog can show 0, 1 or 2 buttons depending on its need. A button can contain an image. If only one button is needed, only one table item must be added. One button will have a centered alignment. Two buttons will have a right alignment. If 0 buttons should be shown, only one table item must be added where the properties "Text" and "Title" should be empty.

A button has the following properties:

| Property | Description |
| :--- | :--- |
| Image | A svg definition for an image. |
| ImagePadding | The padding of the image. |
| MinimalWidth | The minimal width. |
| Text | The text. |
| Title | The internal name. This is needed to support multilingual canvas apps. |
| Type | The button type. Possible values are "Primary" and "Secondary". |

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_Button" which contains the title of the button clicked on.

### cmp_TextStyling
This custom property is of data type "Table" and a record has the following properties:

| Property | Description |
| :--- | :--- |
| Align | The text alignment. |
| ButtonHeight | The height. |
| Color | The color. |
| ID | An unique ID for the table record. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| Padding | The padding. |
| VerticalAlign | The vertical alignment. |

Not all properties are needed in all table records.