# PACo_Nav_C

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://user-images.githubusercontent.com/35654198/235981084-9e19c40d-74f4-4f1a-bdb0-fd2b93e4e88a.png)

This is a responsive canvas component. 

You can use the canvas app "PACo Examples" for a better understanding of, and to experiment with, this canvas component.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_OnSelect | Event | | Boolean | When a navigation item is clicked on. | See the documention on cmp_OnSelect below. |
| cmp_Nav | Data | Input | Table | The navigation items. | See the documention on cmp_Nav below. |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention on cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |

### cmp_Nav
A navigation item has the following properties:

| Property | Description |
| :--- | :--- |
| Disabled | Used to disable the navigation item. |
| ID | The unique number of the navigation item used in the behavior property "cmp_OnSelect". |
| Image | A svg definition for an image for a non-selected navigation item. |
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
| TextBlockHeight | The height of the navigation item. |
