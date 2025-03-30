# PACo_ProgressIndicator_E

This documentation page is related to version: 3.2.0

![image](https://github.com/user-attachments/assets/68a9ca8c-28c6-4ed9-940d-faba6fd08551)

The image above shows an example with, and an example without, text.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_BackgroundColor | Data | Input | Text | The color of the background. | |
| cmp_ColorActive | Data | Input | Text | The color for the current or a previous stage. | |
| cmp_ColorInactive | Data | Input | Text | The color for a next stage. | |
| cmp_CurrentStage | Data | Input | Number | The number of the current stage. Numbering starts at 1. | |
| cmp_Items | Data | Input | Table | The process steps. | See the documention about cmp_Items below. |
| cmp_Offset | Data | Input | Number | The vertical offset when text is shown. | |
| cmp_OnSelect | Event | | None | The event fired when a process step (circle) is clicked on. | See the documentation about cmp_OnSelect below. |
| cmp_ShowText | Data | Input | Boolean | To show the text (or not). | If no text is shown, the progress indicator is centered vertically and the offset is not used.  |
| cmp_TemplateSize | Data | Input | Number | The related property of the gallery used in this canvas component. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Items
A process step has the following properties:

| Property | Description |
| :--- | :--- |
| Clickable | If the process step is clickable or not. |
| ID | An unique number of the process step. Numbering must start at 1 and be sequential. |
| Image | A svg definition for the image. |
| Text | The text to display. |

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_ID" which contains the ID of the process step clicked on.

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
