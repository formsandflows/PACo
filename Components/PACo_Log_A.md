# PACo_Log_A

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

This is a responsive canvas component. 

You can use the canvas app "PACo Examples" for a better understanding of, and to experiment with, this canvas component.

## Custom properties
| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Add | Action | | Boolean | Add a log item to the collection. | See documentation on coll_Log below. |
| cmp_HasImages | Data | Input | Boolean | If images are shown in the log or not. | |
| cmp_Log | Data | Output | Table | The log items. | |
| cmp_Reset | Action | | Boolean | Reset the collection with log items. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention on cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Update | Action | | Boolean | Update a log item in the collection. | |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of canvas component cmp_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Log
A canvas component instance has a collection which is filled with values using the custom property "cmp_Add" and has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID of the log item. |
| Image | A svg definition for the image. Leave it empty if you do not want to show an image. |
| ImagePadding | The padding of the image. |
| Log | The log text. |

### cmp_TextStyling
This custom property is of data type "Record" and has the following properties:

| Property | Description |
| :--- | :--- |
| Align | The vertical alignment. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| TextBlockHeight | The height of the log items. |
