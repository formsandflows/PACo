# PACo_SelectList_A

This documentation page is related to version: 3.0.1

![image](https://github.com/formsandflows/PACo/assets/35654198/67f5c553-d10d-47c1-bea6-0714ab1dc25b)

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Button | Data | Input | Record | The button at the bottom of the panel. | See the documention about cmp_Button below. |
| cmp_OnSelect | Event | | Boolean | When the button is clicked on. | |
| cmp_OnSelectListItem | Event | | Boolean | When a select list item is clicked on. | See the documention about cmp_OnSelectListItem below. |
| cmp_SelectList | Data | Input | Table | The select list items. | See the documention about cmp_SelectList below. |
| cmp_TextStyling | Data | Input | Table | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |
| cmp_Width | Data | Input | Number | The width of the panel. | |

### cmp_Button
The button has the following properties:

| Property | Description |
| :--- | :--- |
| BorderRadius | The radius of the border of the button. |
| Height | The height.|
| Image | A svg definition for an image. An image is not required. |
| ImagePadding | The padding of the image. |
| MinimalWidth | The minimal width. |
| Text | The text. |

### cmp_OnSelectListItem
This custom property contains a required parameter called "cmp_Param_Value" which contains the value of the select list item clicked on.

### cmp_SelectList
A select list item has the following properties:

| Property | Description |
| :--- | :--- |
| Order | The order of the select list item. |
| Value | The value. |

### cmp_TextStyling
This custom property is of data type "Table" and a record has the following properties:

| Property | Description |
| :--- | :--- |
| Align | The horizontal alignment. |
| Color | The color. |
| ID | An unique ID for the section. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| Padding | The padding. |
| TextBlockHeight | The height of the text block. |
| VerticalAlign | The vertical alignment. |

Not all properties are needed in all records.
