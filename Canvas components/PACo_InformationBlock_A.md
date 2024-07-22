# PACo_InformationBlock_A

> [!WARNING]
> This page is a pre-release page. It contains documentation for a future release. Please look in de folder "Archive" for documentation on released versions.

This documentation page is related to version: 3.2.0

## Custom properties
| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_BackgroundColor | Data | Input | Text | The color of the background. | |
| cmp_DefaultHeight | Data | Input | Number | The default label and data height. | |
| cmp_DividerColor | Data | Input | Text | The color of the divider. | |
| cmp_InformationBlock | Data | Input | Table | The data in the information block.. | See documentation on cmp_InformationBlock below. |
| cmp_OnSelect | Event | | None | The event fired when a log item is clicked on. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention on cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Title | Data | Input | Text | The title to show. | |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_InformationBlock
A gallery is used to show data in the panel. Data consists of records. A record has the following properties:

| Property | Description |
| :--- | :--- |
| Clickable | If the record (the data, not the label) is clickable or not. |
| ID | The unique ID of the record. |
| Label | The label text. |
| LabelHeight | The height of the text block of a label. |
| Text | The gallery item text. |
| TextHeight | The height of the text block of a gallery item. |

The LabelHeight and TextHeight properties are not required. A value of 40 is used in case the properties are not defined.

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_ID" which contains the ID of the record clicked on.

### cmp_TextStyling
This custom property is of data type "**Table**" and has the following records:

#### Data

| Property | Description |
| :--- | :--- |
| Align | The horizontal alignment. |
| Color | The color. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| ID | The value: Title |
| Padding | The padding. |
| VerticalAlign | The vertical alignment. |

#### Label

| Property | Description |
| :--- | :--- |
| Align | The horizontal alignment. |
| Color | The color. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| ID | The value: Title |
| Padding | The padding. |
| VerticalAlign | The vertical alignment. |

#### Title

| Property | Description |
| :--- | :--- |
| Align | The horizontal alignment. |
| Color | The color. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| ID | The value: Title |
| Padding | The padding. |
| VerticalAlign | The vertical alignment. |
