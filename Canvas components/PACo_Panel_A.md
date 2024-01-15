# PACo_Panel_A

This documentation page is related to version: 3.0.1

Related video page: https://www.formsandflows.nl/paco/videos/paco_panel_a/

![image](https://github.com/formsandflows/PACo/assets/35654198/ccde7a33-bbb7-429a-be97-37094da8ea76)

The idea is that a panel is shown when an item in a details list is clicked on. This must be configured in the details list. With a panel, normally all data is shown meaning more item properties than the ones shown in the related details list. A vertical scrollbar appears when there is more data to show than fits on the screen.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Button | Data | Input | Record | The button at the bottom of the panel. | See the documention about cmp_Button below. |
| cmp_Commands | Data | Input | Record | The panel commands at the top of the panel. | See the documention about cmp_Commands below. |
| cmp_OnCommandSelect | Event | | Boolean | When a command is clicked on. | See the documention on cmp_OnCommandSelect below. |
| cmp_OnSelect | Event | | Boolean | When the button is clicked on. |
| cmp_Panel | Data | Input | Table | The data in the panel. | See the documention about cmp_Panel below. |
| cmp_TextStyling | Data | Input | Table | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |
| cmp_Width | Data | Input | Number | The width of the panel. | |

### cmp_Button
The panel button has the following properties:

| Property | Description |
| :--- | :--- |
| BorderRadius | The radius of the border of the button. |
| Height | The height. |
| Image | A svg definition for an image. An image is not required. |
| ImagePadding | The padding of the image. |
| MinimalWidth | The minimal width. |
| Text | The text. |

### cmp_Commands
A panel command has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID (number) of the panel command bar item. |
| Image | A svg definition for the image. |
| ImagePadding | The padding of the image. |
| Text | The text. |

A maximum of 2 panel commands is supported!

When the property "Text" has no value, the related panel command is not shown.

When the property "Text" has no value for both commands, the panel command bar is not shown.

### cmp_OnCommandSelect
This custom property contains a required parameter called "cmp_Param_CommandID" which contains the ID of the panel command clicked on.

### cmp_Panel
A gallery is used to show data in the panel. Data consists of records. A record has the following properties:

| Property | Description |
| :--- | :--- |
| Label | The label text. |
| LabelHeight | The height of the text block of a label. |
| Text | The gallery item text. |
| TextHeight | The height of the text block of a gallery item. |

The LabelHeight and TextHeight properties are not required. A value of 40 is used in case the properties are not defined.

### cmp_TextStyling
This custom property is of data type "Table" and a record has the following properties:

| Property | Description |
| :--- | :--- |
| Align | The horizontal alignment. |
| Color | The color. |
| ID | An unique ID for the table record. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| TextBlockHeight | The height of the text block. |
| VerticalAlign | The vertical alignment. |

Not all properties are needed in all table records.
