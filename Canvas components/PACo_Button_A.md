# PACo_Button_A

> [!CAUTION]
> This documentation page is currently in the process of being upgraded to canvas component version 3.1.0 which will be released very soon.

This documentation page is related to version: 3.1.0

Related video page: https://www.formsandflows.nl/paco/videos/paco_button_a/

![PACo_Button_A](https://github.com/formsandflows/PACo/assets/35654198/00c5b60c-c0e5-4b86-ba9a-526164414d5f)

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Button | Data | Input | Record | Button properties. | See the documention about cmp_Button below. |
| cmp_Disabled | Data | Input | Boolean | If the button is disabled or not. | |
| cmp_OnSelect | Event | | Boolean | When the button is clicked on and not disabled. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Tooltip | Data | Input | Text | The tooltip. | |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Width | Data | Output | Number | The actual width of the button. | See the documention about cmp_Width below. |

### cmp_Button
This custom property is of data type "Record" and has the following properties:

| Property | Description |
| :--- | :--- |
| Border | If a border must be shown. This only applies to a button of type "Secondary". |
| BorderRadius | The radius of the border of the button. |
| Image | A svg definition for the image. Leave it empty if you do not want to show an image. |
| ImagePadding | The padding of the image. |
| MinimalWidth | The minimal width. |
| Text | The text. |
| Type | The button type. Possible values are "Primary" and "Secondary". |

The first button shown in the screenshot above is of type "Primary". The second button is of type "Secondary". The third is of type "Primary" and is disabled. The fourth is of type "Secondary" and disabled.

### cmp_TextStyling
This custom property has the following properties:

| Property | Description |
| :--- | :--- |
| Color | The color. |
| Font | The font. |
| FontSize | The font size. |

### cmp_Width
The actual width of the button is determined by several factors:
- The minimal width as defined in the custom property "cmp_Button".
- The length of the text.
- If there is an image to shown as defined in the custom property "cmp_Button".
- The image padding as defined in the custom property "cmp_Button".

The image padding is always shown as space to the left and the right in the button.

**!! This custom property must be set as the width of the canvas component instance by using:** `Self.cmp_Width`
