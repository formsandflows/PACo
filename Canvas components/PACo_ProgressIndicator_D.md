# PACo_ProgressIndicator_D

> [!CAUTION]
> This documentation page is currently in the process of being upgraded to canvas component version 3.1.0 which will be released very soon.

This documentation page is related to version: 3.1.0



## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_ColorActive | Data | Input | Text | The color for the current or a previous stage. | |
| cmp_ColorInactive | Data | Input | Text | The color for an inactive or next stage. | |
| cmp_CurrentStage | Data | Input | Number | The number of the current stage. Numbering starts at 1. | |
| cmp_Items | Data | Input | Table | The process steps. | See the documention about cmp_Items below. |
| cmp_Offset | Data | Input | Number | The vertical offset when text is shown. | |
| cmp_ShowText | Data | Input | Boolean | To show the text (or not). | If no text is shown, the progress indicator is centered vertically and the offset is not used. |
| cmp_TemplateSize | Data | Input | Number | The related property of the gallery used in this canvas component. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Items
A process step has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique number of the process step. Numbering must start at 1 and be sequential. |
| Skip | If the process step must be skipped (inactive) or not. |
| Text | The text to display. |

### cmp_TextStyling
This custom property has the following properties:

| Property | Description |
| :--- | :--- |
| Color | The color. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| Height | The height. |
| Padding | The padding. |
| VerticalAlign | The vertical alignment. |
