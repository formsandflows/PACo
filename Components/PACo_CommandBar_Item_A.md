# PACo_CommandBar_Item_A

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://user-images.githubusercontent.com/35654198/235982444-ff55c19b-41fd-4bba-aa9f-5037f2296c2a.png)

This is a responsive canvas component. The width of the canvas component instance must be configured as: `Self.cmp_Width`

You can use the canvas app "PACo Examples" for a better understanding of, and to experiment with, this canvas component.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Image | Data | Input | Text | A svg definition for the image. | |
| cmp_ImagePadding | Data | Input | Number | The padding of the image. | |
| cmp_OnSelect | Event | | Boolean | When the command bar item is clicked on. | |
| cmp_Text | Data | Input | Text | The text. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention on cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme to use. | See the documention on theming. |
| cmp_Width | Data | Output | Number | The actual width of the command bar item. | See the documention on cmp_Width below. |

### cmp_TextStyling
This custom property is of data type "Record" and has the following properties:

| Property | Description |
| :--- | :--- |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |

### cmp_Width
The actual width of the command bar item is determined by several factors:
- The width of the image.
- The length of the text to show.
- The image padding as defined in the custom property "cmp_ImagePadding".
