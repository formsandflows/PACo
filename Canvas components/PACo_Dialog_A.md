# PACo_Dialog_A

> [!WARNING]
> This page is a pre-release page. It contains documentation for a future release. Please look in de folder "Archive" for documentation on released versions.

This documentation page is related to version: 3.2.0

Related video page: https://www.formsandflows.nl/paco/videos/paco_dialog_a/

![image](https://github.com/formsandflows/PACo/assets/35654198/ad42c67b-c4c2-4068-ad4d-2b3f88f36088)

When using variables for the input properties, one dialog component can be used for multiple situations. This is implemented in the canvas app "PACoCo".

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_BackgroundColor | Data | Input | Text | The color of the background. | |
| cmp_Buttons | Data | Input | Table | The buttons to show. | See the documention about cmp_Buttons below. |
| cmp_Message | Data | Input | Text | The message of the dialog in plain text. | |
| cmp_MessageHTML | Data | Input | Text | The message of the dialog in HTML. | |
| cmp_OnSelect | Event | | None | The event fired when a button is clicked on. | |
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
| Border | If a border must be shown. This only applies to a button of type "Secondary". |
| BorderRadius | The radius of the border of the button. |
| Height | The height. |
| Image | A svg definition for an image. |
| ImagePadding | The padding of the image. |
| MinimalWidth | The minimal width. |
| Text | The text. |
| Title | The internal name. This is needed to support multilingual canvas apps. |
| Type | The button type. Possible values are "Primary" and "Secondary". |

For the height of buttons, only the height property of the first button record is used.

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_Button" which contains the title of the button clicked on.

### cmp_TextStyling
This custom property is of data type "**Table**" and has the following records:

#### Button

| Property | Description |
| :--- | :--- |
| ColorPrimary | The color for button of type "Primary". |
| ColorSecondary | The color for button of type "Secondary". |
| ID | The value: Button |
| Font | The font. |
| FontSize | The font size. |

#### Message

| Property | Description |
| :--- | :--- |
| Align | The text alignment. |
| Color | The color. |
| ID | The value: Message |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| Padding | The padding. |
| VerticalAlign | The vertical alignment. |

#### MessageHTML

| Property | Description |
| :--- | :--- |
| Color | The color. |
| ID | The value: MessageHTML |
| Font | The font. |
| FontSize | The font size. |
| Padding | The padding. |

#### Title

| Property | Description |
| :--- | :--- |
| Align | The text alignment. |
| Color | The color. |
| ID | The value: Title |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| Padding | The padding. |
