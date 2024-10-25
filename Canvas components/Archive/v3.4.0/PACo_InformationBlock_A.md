# PACo_InformationBlock_A

This documentation page is related to version: 3.4.0

![image](https://github.com/user-attachments/assets/e57ec752-4e9c-4cd5-a5ae-ad12c11c6e32)

## Custom properties
| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_AutoHeight | Data | Input | Boolean | To set auto height or not. | Auto height is configured on all "Text label" controls (Title, Label and Text block). |
| cmp_BackgroundColor | Data | Input | Text | The color of the background. | |
| cmp_ChevronStyling | Data | Input | Record | Chevron properties. | See the documention on cmp_ChevronStyling below. |
| cmp_Collapsed | Data | Input | Boolean | If the information block is collapsed or not. | |
| cmp_DefaultHeight | Data | Input | Number | The default label and data height. | |
| cmp_DividerColor | Data | Input | Text | The color of the divider. | |
| cmp_InformationBlock | Data | Input | Table | The data in the information block.. | See documentation on cmp_InformationBlock below. |
| cmp_OnSelect | Event | | None | The event fired when a log item is clicked on. | |
| cmp_OnSelectChevron | Event | | None | The event fired when the chevron is clicked on. | |
| cmp_TextStyling | Data | Input | Table | Text properties. | See the documention on cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Title | Data | Input | Text | The title to show. | |
| cmp_TitleHeight | Data | Output | Number | | |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_ChevronStyling
This custom property has the following properties:

| Property | Description |
| :--- | :--- |
| Color | The color. |
| ImageCollapsed | The svg to show when collapsed. |
| ImageNotCollapsed | The svg to show when not collapsed. |
| Padding | The padding. |

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
| FontStyle | One of the following options: Default, Italic, Strikethrough, Underline |
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
| FontStyle | One of the following options: Default, Italic, Strikethrough, Underline |
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
| FontStyle | One of the following options: Default, Italic, Strikethrough, Underline |
| FontWeight | The font weight. |
| ID | The value: Title |
| Padding | The padding. |
| VerticalAlign | The vertical alignment. |
