# PACo_Panel_A

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://user-images.githubusercontent.com/35654198/235981450-7e4a2fd9-d4cc-436b-9847-ea35c39804a2.png)

A panel is shown when an item in the details list is clicked on. This must be configured in the details list component! With a panel, normally all data is shown meaning more item properties than the ones shown in the details list. A vertical scrollbar appears when there is more data to show than fits on the screen.

You can use the canvas app "PACo Examples" for a better understanding of, and to experiment with, this canvas component.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Button | Data | Input | Record | The button at the bottom of the panel. | See the documention on cmp_Button below. |
| cmp_Commands | Data | Input | Record | The panel command bar items at the top of the panel. | See the documention on cmp_Commands below. |
| cmp_OnCommandSelect | Event | | Boolean | When a command bar item is clicked on. | |
| cmp_OnSelect | Event | | Boolean | When the button is clicked on. |
| cmp_Records | Data | Input | Table | The data in the panel. | See the documention on cmp_Records below. |
| cmp_TextStyling | Data | Input | Table | Text properties. | See the documention on cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of component cmp_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |
| cmp_Width | Data | Input | Number | The the width of the panel. | |

### cmp_Button

The panel button has the following properties:

| Property | Description |
| :--- | :--- |
| Image | A svg definition for an image. An image is not required. |
| ImagePadding | The padding of the image. |
| MinimalWidth | The minimal width of the button. |
| Text | The text to display in the button. |

### cmp_Commands
A panel command bar item has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID (number) of the command bar item. |
| Image | A svg definition to be used as an icon. |
| ImagePadding | The padding of the images. |
| Text | The text to display in the related label control. |

A maximum of 2 commands is supported!

When the property "Text" has no value, the related panel command bar item is not shown.

### cmp_Records
A gallery is used to show data in the panel. Data consists of records. A record has the following properties:

| Property | Description |
| :--- | :--- |
| Label | The label text. |
| LabelHeight | The height of the label. |
| Text | The gallery item text. |
| TextHeight | The height of the gallery item. |

The LabelHeight and TextHeight properties are not required. A value of 40 is used in case the properties are not defined.

### cmp_OnCommandSelect
This custom property contains a required parameter called "cmp_Param_CommandID" which contains the ID of the Panel command bar item clicked on.

### cmp_TextStyling
This custom property is of data type "Table" and a record has the following properties:

| Property | Description |
| :--- | :--- |
| ButtonHeight | The button height. |
| ID | An unique ID for the section. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |

Not all properties are used by all controls.
