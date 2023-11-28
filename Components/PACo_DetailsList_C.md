# PACo_DetailsList_C

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://user-images.githubusercontent.com/35654198/235979572-89783b98-c265-44c7-b2ef-e3f8158662b7.png)

Per item, up to 3 fields can be shown:
* Title which is based on a label control.
* Subtitle which is based on a label control.
* HTML which is based on a html control.

You can use the canvas app "PACo Examples" for a better understanding of, and to experiment with, this canvas component.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_DetailsList | Data | Input | Table | The details list items. | See the documention on cmp_DetailsList below. |
| cmp_OnCheck | Event | | Boolean | When the item checkbox is clicked on and the checkbox is unchecked. | |
| cmp_OnUncheck | Event | | Boolean | When the item checkbox is clicked on and the checkbox is checked. | |
| cmp_ResetCheckbox | Data | Input | Boolean | To reset the checkbox of all details list items. | |
| cmp_ShowCheckbox | Data | Input | Boolean | To show the checkbox for details list items or not. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention on cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The themee. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization to use. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | #0078d4 |

### cmp_DetailsList
To have a more consistent naming with the other details list components in PACo-Core, several properties contain the text "Column" which can be read a "Field".

The properties have "Small" in their naming so 1 collection can be used to be used by this canvas component as well as a canvas component to used when the screen has more width. With this setup, the first 3 columns can differ instead of having to be the same.

For each details list item, the following properties must be available:
- Column1SmallColor
- Column1SmallFontSize
- Column1SmallFontWeight
- Column1SmallText
- Column2SmallColor
- Column2SmallFontSize
- Column2SmallFontWeight
- Column2SmallText
- Column3SmallFontSize
- Column3SmallText
- SmallFill
- SmallFillSelected

Only the use of a collection which contains the details list items is supported! Dataverse tables, SharePoint lists, ... can thus not directly be connected to the property "cmp_DetailsList".

The collection to display the details list items must have the additional required property:

| Property | Description |
| :--- | :--- |
| RecordID | The unique ID of the item. This property is of type "Text".  |
| Selected | This property must be set when checking/unchecking a details list item. This property is of type "Boolean". |

### cmp_OnCheck
This custom property contains a required parameter called "cmp_Param_RecordID" which contains the unique ID of the selected item (Record ID).

### cmp_OnUncheck
This custom property contains a required parameter called "cmp_Param_RecordID" which contains the unique ID of the selected item (Record ID).

### cmp_TextStyling
This custom property is of data type "Record" and has the following properties:

| Property | Description |
| :--- | :--- |
| BodyHeight | An additional height for all detail list items. |
| Font | The font. |
| TextBlockHeight | The height of the detail list items. |
