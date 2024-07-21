# PACo_ProgressIndicator_Shimmer_A

> [!WARNING]
> This page is a pre-release page. It contains documentation for a future release. Please look in de folder "Archive" for documentation on released versions.

This documentation page is related to version: 3.2.0

![image](https://github.com/formsandflows/PACo/assets/35654198/7f764760-d0f8-4468-9919-cada10953cae)

The image above shows an example with, and an example without, text.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_BackgroundColor | Data | Input | Text | The color of the background. | |
| cmp_NumberOfItems | Data | Input | Number | The number of steps. |  |
| cmp_Offset | Data | Input | Number | The vertical offset when the text placeholder is shown. |  |
| cmp_ShimmerColor | Data | Input | Text | The color of the shimmer. | |
| cmp_ShowText | Data | Input | Boolean | To show the text placeholder (or not). |  |
| cmp_TemplateSize | Data | Input | Number | The related property of the gallery used in this canvas component. |  |
| cmp_TextStyling | Data | Input | Record | Text placeholder properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_TextStyling
This custom property has the following properties:

| Property | Description |
| :--- | :--- |
| Height | The height. |
