# PACo_Tile_A

This documentation page is related to version: 3.0.0

Related video page: https://www.formsandflows.nl/paco/videos/paco_tile_a/

![image](https://github.com/formsandflows/PACo/assets/35654198/0a09c772-fe16-41e9-a16e-50ad34c73318)

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_PercentageTextHeight | Data | Input | Number | The percentage of the height for the text section. | |
| cmp_Text | Data | Input | Text | The text to shown in the upper section of the tile. | |
| cmp_TextStyling | Data | Input | Table | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Value | Data | Input | Number | The value to show in the lower section of the tile. | |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_TextStyling
This custom property is of data type "Table" and a record has the following properties:

| Property | Description |
| :--- | :--- |
| Align | The horizontal alignment. |
| Color | The color. |
| ID | An unique ID for the section (Text or Value). |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| Padding | The padding. |
| VerticalAlign | The vertical alignment. |
