# PACo_ProgressIndicator_B

This documentation page is related to version: 3.0.0

Related video page: https://www.formsandflows.nl/paco/videos/paco_progressindicator_b/

![image](https://github.com/formsandflows/PACo/assets/35654198/4d57e4fb-e8da-45da-8a6d-e69941bbef78)

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_ColorActive | Data | Input | Text | The color for the current or a previous stage. | |
| cmp_ColorInactive | Data | Input | Text | The color for an inactive or next stage. | |
| cmp_CurrentStage | Data | Input | Number | The number of the current stage. Numbering starts at 1. | |
| cmp_Items | Data | Input | Table | The process steps. | See the documention about cmp_Items below. |
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
This custom property is of data type "Record" and has the following properties:

| Property | Description |
| :--- | :--- |
| Color | The color. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| Padding | The padding. |
| VerticalAlign | The vertical alignment. |
