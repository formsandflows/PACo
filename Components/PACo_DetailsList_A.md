# PACo_DetailsList_A

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://user-images.githubusercontent.com/35654198/235978809-ca5d0c95-df32-4ea2-b304-88520dbdd83f.png)

This is a responsive canvas component. A horizontal scroll appears when the width of the details list is greater than the width of the screen.

You can use the canvas app "PACo Examples" for a better understanding of, and to experiment with, this canvas component.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_DetailsList | Data | Input | Table | The details list items. | See the documention on cmp_DetailsList below. |
| cmp_Header | Data | Input | Record | The details list header. | See the documention on cmp_Header below. |
| cmp_OnCheck | Event | | Boolean | When the item checkbox is clicked on ans the checkbox is unchecked. | |
| cmp_OnCheckAll | Event | | Boolean | When the checkbox in the header is clicked on and the checkbox is unchecked. | |
| cmp_OnHeaderSelect | Event | | Boolean | When a header column is clicked on. | |
| cmp_OnSelect | Event | | Boolean | When a details list item is clicked on. | |
| cmp_OnUncheck | Event | | Boolean | When the item checkbox is clicked on ans the checkbox is checked. | |
| cmp_OnUncheckAll | Event | | Boolean | When the checkbox in the header is clicked on and the checkbox is checked. | |
| cmp_ResetCheckbox | Data | Input | Boolean | To reset the checkbox of all items in the details list. | |
| cmp_ResetCheckboxHeader | Data | Input | Boolean | To reset the checkbox in the header. | |
| cmp_ShowCheckbox | Data | Input | Boolean | To show the checkbox for details list items or not. | |
| cmp_ShowCheckboxHeader | Data | Input | Boolean | To show the checkbox in the header or not. | |
| cmp_SortingColumn | Data | Input | Text | The sorting column. | |
| cmp_SortingDirection | Data | Input | Text | The sorting direction. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention on cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of component cmp_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_DetailsList
This canvas component is configured to have a maximum of 20 columns. To be able to display the items, a collection with a pre-defined set of required(!) properties must be used. This was needed to make this canvas component a generic canvas component.

For each column, the following properties must be available:
- Column#Align
- Column#Color
- Column#ColorSelected
- Column#Fill
- Column#FillSelected
- Column#FontWeight
- Column#Text
- Column#Tooltip
- Column#VerticalAlign
, where # is the number of the column. These properties relate to the control properties of the label control in the gallery used to show the data.

Only the use of a collection which contains the details list items is supported! Dataverse tables, SharePoint lists, ... can thus not directly be connected to the custom property "cmp_DetailsList".

The collection to display the details list items must have 2 additional required properties:

| Property | Description |
| :--- | :--- |
| RecordID | The unique ID of the details list item. This property is of type "Text". |
| Selected | This property must be set when checking/unchecking a details list item. This property is of type "Boolean". |

**!! Attention: All 20 columns must be defined.**

### cmp_Header
Every header column has its own subrecord. A header column has the following properties:

| Property | Description |
| :--- | :--- |
| Sortable | This determines if the related header column can be used for sorting. |
| Text | The text to show in the related label control. |
| Width | The width of the related label control. |

The width of a header can thus be configured but is fixed when using the app. It is possible to define the header outside the canvas app so it can be changed without changing the canvas app. This is a recommended approach.

If the total width of all columns together is larger than the width of this details list canvas component, a horizontal scrollbar is shown.

This canvas component is configured to have a maximum of 20 columns. When a column shoud not be used:
- set the property "Text" to an empty string ("").
- set the property "Width" to 0.

, for the related header column.

**!! Attention: All 20 columns must be defined.**

### cmp_OnCheck
This custom property contains a required parameter called "cmp_Param_RecordID" which contains the unique ID of the selected details list item (Record ID).

### cmp_OnHeaderSelect
This custom property contains a required parameter called "cmp_Param_Column" which contains the text of the column clicked on.

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_RecordID" which contains the unique ID of the selected details list item (Record ID).

### cmp_OnUncheck
This custom property contains a required parameter called "cmp_Param_RecordID" which contains the unique ID of the selected details list item (Record ID).

### cmp_TextStyling
This custom property is of data type "Record" and has the following properties:

| Property | Description |
| :--- | :--- |
| Font | The font. |
| FontSize | The font size. |
| HeaderHeight | The height of the header. |
| TextBlockHeight | The height of the detail list items. |
