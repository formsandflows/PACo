# PACo_Button_A

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://user-images.githubusercontent.com/35654198/235982340-10a1d796-453c-45cd-9c4d-4aacc4de5723.png)

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Button | Data | Input | Record | Button properties. | See the documention on cmp_Button below. |
| cmp_Disabled | Data | Input | Boolean | If the button is disabled or not. | |
| cmp_OnSelect | Event | | Boolean | When the button is clicked on and not disabled. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention on cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Width | Data | Output | Number | The actual width of the button. | See the documention on cmp_Width below. |

### cmp_Button
This custom property is of data type record and has the following properties:

| Property | Description |
| :--- | :--- |
| Image | A svg definition for the image. Leave it empty if you do not want to show an image. |
| ImagePadding | The padding of the image. |
| MinimalWidth | The minimal width of the button. |
| Text | The text to display in the button. |
| Type | The button type. Possible values are: Primary, Secondary. |

This first button shown in the screenshot above is of type "Primary" and the second button of type "Secondary".

### cmp_TextStyling
This custom property is of data type record and has the following properties:

| Property | Description |
| :--- | :--- |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |

### cmp_Width
The actual width of the button is determined by several factors:
- The minimal width as defined in the custom property "cmp_Button".
- The length of the text to show.
- If an image must be shown as defined in the custom property "cmp_Button".
- The image padding as defined in the custom property "cmp_Button".

The image padding is always shown as space to the left and the right in the button.
