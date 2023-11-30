# PACo_SelectList_A

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://github.com/formsandflows/PACo/assets/35654198/8ee22ec2-5d31-4fc2-b996-287d5bc77b28)

A select list is used when a selected from one set of values must be made. This component also has a search box which filter the data on values containing the text types in the search box.

This canvas component has its "OnReset" property configured. When a canvas component instance is reset, the text shown in the search box and button is reset.

You can use the canvas app "PACo Examples" for a better understanding of, and to experiment with, this canvas component.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Button | Data | Input | Record | The button at the bottom of the panel. | See the documention on bcmp_Btton below. |
| cmp_OnSelect | Event | | Boolean | When the button is clicked on. | |
| cmp_OnSelectListItem | Event | | Boolean | When a select list item is clicked on. | See the documention on cmp_OnSelectListItem below. |
| cmp_SelectList | Data | Input | Table | The select list items. | See the documention on cmp_SelectList below. |
| cmp_TextStyling | Data | Input | Table | Text properties. | See the documention on cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of canvas component cmp_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |
| cmp_Width | Data | Input | Number | The width of the panel. | |

### cmp_Button
The button has the following properties:

| Property | Description |
| :--- | :--- |
| Height | The height.|
| Image | A svg definition for an image. An image is not required. |
| ImagePadding | The padding of the image. |
| MinimalWidth | The minimal width. |
| Text | The text. |

### cmp_OnSelectListSelect
This custom property contains a required parameter called "cmp_Param_Value" which contains the value of the select list item clicked on.

### cmp_SelectList
A gallery is used to show data for the select list. Data consists of records. A record has the following properties:

| Property | Description |
| :--- | :--- |
| Value | The value to show. |

### cmp_TextStyling
This custom property is of data type "Table" and a record has the following properties:

| Property | Description |
| :--- | :--- |
| Height | The height of the related element. |
| ID | An unique ID for the section. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |

The height of the search box must include the whitespace at the top and bottom of 10 each.

Not all properties are needed in all records.
