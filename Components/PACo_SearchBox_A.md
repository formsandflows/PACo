# PACo_SearchBox_A

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://user-images.githubusercontent.com/35654198/235981615-a3eba4ed-f2b6-4cbc-be71-c3661f3cc59f.png)

This is a responsive canvas component.

The search box can be used to filter the items shown in a details list.

This canvas component has its "OnReset" property configured. When a canvas component instance is reset, the text shown in the search box reset.

You can use the canvas app "PACo Examples" for a better understanding of, and to experiment with, this canvas component.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_HintText | Data | Input | Text | The hint text. | |
| cmp_Images | Data | Input | Table | Properties of the images. | See the documention on cmp_Images below. |
| cmp_Text | Data | Output | Text | Contains the text typed into the search box. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention on cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of component cmp_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Images
This custom property is of data type "Table" and a record has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID for the image. |
| Image | A svg definition for the image. |
| ImagePadding | The padding of the image. |

### cmp_TextStyling
This custom property is of data type "Record" and has the following properties:

| Property | Description |
| :--- | :--- |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
