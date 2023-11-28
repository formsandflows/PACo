# PACo_Nav_B

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://user-images.githubusercontent.com/35654198/235980799-970ab7a7-b4e5-4b4f-9270-fdead5e0ad97.png)

You can use the canvas app "PACo Examples" for a better understanding of, and to experiment with, this canvas component.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Nav | Data | Input | Table | The navigation items. | See the documention on cmp_Nav below. |
| cmp_OnSelect | Event | | Boolean | When a navigation item is clicked on. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention on cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme to use. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization to use. | See the documention of component cmp_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### Navigation menu items
A navigation item has the following properties:

| Property | Description |
| :--- | :--- |
| AlignWithImage | Used when not having an image and to allign the text with navigation items which do have an image. |
| Disabled | Used to disable the navigation item. |
| ID | The unique number of the navigation item used in the custom property "cmp_OnSelect". |
| Image | A svg definition for the image for a non-selected navigation item. |
| ImagePadding | The padding of the image. |
| ImageSelected | A svg definition for the image for a selected navigation item. |
| Order | The order of the item in the navigation. |
| Screen | The screen object to navigate to. |
| Text | The text. |

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_NavID" which contains the ID of the navigation item clicked on.

### cmp_TextStyling
This custom property is of data type "Record" and has the following properties:

| Property | Description |
| :--- | :--- |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| TextBlockHeight | The height of the navigation items. |
