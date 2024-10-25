# PACo_Breadcrumb_A

This documentation page is related to version: 3.4.0

![image](https://github.com/user-attachments/assets/27104b34-e4a8-4abd-8a96-a76b7f64985a)

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_BackgroundColor | Data | Input | Text | The color of the background. | |
| cmp_Breadcrumb | Data | Input | Table | The breadcrumb items. | See the documention about cmp_Breadcrumb below. |
| cmp_OnSelect | Event | | None | The event fired when a breadcrumb item is clicked on. | See the documention about cmp_OnSelect below. |
| cmp_Seperator | Data | Input | Record | The seperator between breadcrumb items. | See the documention about cmp_Seperator below. |
| cmp_ShowUnderline | Data | Input | Boolean | To show the underline or not. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Breadcrumb
A breadcrumb item has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID (number) of the breadcrumb item. |
| Text | The text. |
| TextPaddingLeft | The padding left of the text. |
| TextPaddingRight | The padding right of the text. |

This component allows for up to 5 breadcrumb items.

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_LevelID" which contains the ID of the breadcrumb item (level) clicked on.

### cmp_Seperator
A seperator has the following properties:

| Property | Description |
| :--- | :--- |
| Image | A svg definition for the image. |
| Margin | The margin. |
| Padding | The padding. |

### cmp_TextStyling
This custom property has the following properties:

| Property | Description |
| :--- | :--- |
| Color | The color. |
| Font | The font. |
| FontSize | The font size. |
