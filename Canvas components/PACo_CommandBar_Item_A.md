# PACo_CommandBar_Item_A

This documentation page is related to version: 3.0.1

Related video page: https://www.formsandflows.nl/paco/videos/paco_commandbar_item_a/

![image](https://user-images.githubusercontent.com/35654198/235982444-ff55c19b-41fd-4bba-aa9f-5037f2296c2a.png)

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Image | Data | Input | Text | A svg definition for the image. | |
| cmp_ImagePadding | Data | Input | Number | The padding of the image. | |
| cmp_OnSelect | Event | | Boolean | When the command bar item is clicked on. | |
| cmp_Text | Data | Input | Text | The text. | |
| cmp_TextPaddingLeft | Data | Input | Number | The padding left of the text. | |
| cmp_TextPaddingRight | Data | Input | Number | The padding right of the text. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme to use. | See the documention on theming. |
| cmp_Width | Data | Output | Number | The actual width of the command bar item. | See the documention about PACo_Width below. |

### cmp_TextStyling
This custom property is of data type "Record" and has the following properties:

| Property | Description |
| :--- | :--- |
| Color | The color. |
| Font | The font. |
| FontSize | The font size. |

### cmp_Width
The actual width of the command bar item is determined by several factors:
- The width of the image.
- The length of the text to show.
- The image padding as defined in the custom property "cmp_ImagePadding".

**!! This custom property must be set as the width of the canvas component instance:** `Self.cmp_Width`
