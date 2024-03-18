# PACo_Info_A

> [!CAUTION]
> This documentation page is currently in the process of being upgraded to canvas component version 3.1.0 which will be released very soon.

This documentation page is related to version: 3.1.0



## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Button | Data | Input | Record | The button to show. | See the documention about cmp_Button below. |
| cmp_Height | Data | Input | Number | The height. | The height of the info-box. This includes 2 times the visualization size. |
| cmp_Image | Data | Input | Text | A svg definition for the pointer. | See the documention about cmp_Image below. |
| cmp_Image_Offset | Data | Input | Number | The image offset. | See the documention about cmp_Image_Offset below. |
| cmp_Location | Data | Input | Text | The location of the pointer. | See the documention about cmp_Location below. |
| cmp_Message | Data | Input | Text | The message of the dialog in plain text. |  |
| cmp_MessageHTML | Data | Input | Text | The message of the dialog in HTML. |  |
| cmp_OnSelect | Event |  | Boolean | When a button is clicked on. |  |
| cmp_TextStyling | Data | Input | Table | Text properties. |  |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Title | Data | Input | Text | The title |  |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |
| cmp_Width | Data | Input | Number | The width. | The width of the info-box. This includes 2 times the visualization size. |
| cmp_X | Data | Input | Number | The reference X-position. | This is the X value of the top-left coordinate of the info-box. The visualization size of 10 has to be taken into account. |
| cmp_Y | Data | Input | Number | The reference Y-position. | This is the Y value of the top-left coordinate of the info-box. The visualization size of 10 has to be taken into account. |

### cmp_Button
The button has the following properties:

| Property | Description |
| :--- | :--- |
| Border | To show a border (or not). |
| BorderRadius | The radius of the border of the button. |
| Height | The height.|
| Image | A svg definition for an image. An image is not required. |
| ImagePadding | The padding of the image. |
| MinimalWidth | The minimal width. |
| Text | The text. |

### cmp_Image
The pointer to use will (normally) differ per location.

### cmp_Image_Offset
The offset related to the X or Y position. Which to use (X or Y) depends on the location.

### cmp_Location
The location determines where the pointer (image) is shown.

There are 4 locations:
- Left
- Right
- Top
- Bottom
