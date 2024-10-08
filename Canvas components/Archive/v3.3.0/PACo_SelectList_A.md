# PACo_SelectList_A

This documentation page is related to version: 3.3.0

Related video page: https://www.formsandflows.nl/paco/videos/paco_selectlist_a/

![image](https://github.com/user-attachments/assets/585c8c33-6c76-4c40-9954-12de5fb07736)

This canvas component has its "OnReset" property configured. When a canvas component instance is reset, the text input control is reset.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_BackgroundColor | Data | Input | Text | The color of the background. | |
| cmp_BackgroundColorSearchBox | Data | Input | Text | The color of the search box background. | |
| cmp_BackgroundColorList | Data | Input | Text | The color of the list background. | |
| cmp_Button | Data | Input | Record | The button at the bottom of the panel. | See the documention about cmp_Button below. |
| cmp_DividerColor | Data | Input | Text | The color of the divider. | |
| cmp_IconColor | Data | Input | Text | The color of the icons. | |
| cmp_OnSelect | Event | | None | The event fired when the button is clicked on. | |
| cmp_OnSelectListItem | Event | | None | The event fired when a select list item is clicked on. | See the documention about cmp_OnSelectListItem below. |
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
| Border | If a border must be shown. This only applies to a button of type "Secondary". |
| BorderRadius | The radius of the border of the button. |
| Height | The height.|
| Image | A svg definition for an image. An image is not required. |
| ImagePadding | The padding of the image. |
| MinimalWidth | The minimal width. |
| Text | The text. |
| Type | The button type. Possible values are "Primary" and "Secondary". |

### cmp_OnSelectListItem
This custom property contains a required parameter called "cmp_Param_Value" which contains the value of the select list item clicked on.

### cmp_SelectList
A select list item has the following properties:

| Property | Description |
| :--- | :--- |
| Order | The order of the select list item. |
| Value | The value. |

### cmp_TextStyling
This custom property is of data type "**Table**" and has the following records:

#### Button

| Property | Description |
| :--- | :--- |
| Color | The color. |
| ID | The value: Button |
| Font | The font. |
| FontSize | The font size. |

#### Search

| Property | Description |
| :--- | :--- |
| Align | The horizontal alignment. |
| Color | The color. |
| ID | The value: Search |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| Padding | The padding. |
| TextBlockHeight | The height of the text block. |

#### SelectListItem

| Property | Description |
| :--- | :--- |
| Align | The horizontal alignment. |
| Color | The color. |
| ID | The value: SelectListItem |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| Padding | The padding. |
| TextBlockHeight | The height of the text block. |
| VerticalAlign | The vertical alignment. |
