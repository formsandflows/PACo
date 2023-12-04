# PACo_HeaderLanguagesMenu_A

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

You can use the canvas app "PACo Examples" for a better understanding of, and to experiment with, this canvas component.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Languages | Data | Input | Table | The languages. | See the documention on cmp_Languages below. |
| cmp_OnSelect | Event | | Boolean | When a language is clicked on. | See the documention on cmp_OnSelect below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Languages
A language has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID (text) of the language. |
| Image| A svg definition for the image. |
| ImagePadding | The padding of the image. |

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_LanguageID" which contains the ID of the language clicked on.
