# PACo_DetailsList_A

This documentation page is related to version: 3.0.0

Related video page: https://www.formsandflows.nl/paco/videos/paco_detailslist_a/

![image](https://github.com/formsandflows/PACo/assets/35654198/960c6c66-f08d-438e-a103-a01e1d193004)

A horizontal scroll appears when the width of the details list is greater than the available width on the screen.

This canvas component has its "OnReset" property configured. When a canvas component instance is reset, the checkboxes in the header and of detail list items are reset.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_DetailsList | Data | Input | Table | The details list items. | See the documention about cmp_DetailsList below. |
| cmp_Header | Data | Input | Record | The details list header. | See the documention about cmp_Header below. |
| cmp_OnCheck | Event | | Boolean | When the details list item checkbox is clicked on and the checkbox is unchecked. | See the documention about cmp_OnCheck below. |
| cmp_OnCheckAll | Event | | Boolean | When the checkbox in the header is clicked on and the checkbox is unchecked. | |
| cmp_OnHeaderSelect | Event | | Boolean | When a header column is clicked on. | See the documention on cmp_OnHeaderSelect below. |
| cmp_OnSelect | Event | | Boolean | When a details list item is clicked on. | See the documention on cmp_OnSelect below. |
| cmp_OnUncheck | Event | | Boolean | When the details list item checkbox is clicked on and the checkbox is checked. | See the documention about cmp_OnUncheck below. |
| cmp_OnUncheckAll | Event | | Boolean | When the checkbox in the header is clicked on and the checkbox is checked. | |
| cmp_ShowCheckbox | Data | Input | Boolean | To show the checkbox for details list items or not. | |
| cmp_ShowCheckboxHeader | Data | Input | Boolean | To show the checkbox in the header or not. | |
| cmp_SortingColumn | Data | Input | Text | The sorting column. | |
| cmp_SortingDirection | Data | Input | Text | The sorting direction. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
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

The collection which contains the details list items must have 2 additional required properties:

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
| Text | The text in the related label control. |
| Width | The width of the related label control. |

The width of a header can thus be configured but is fixed when using the app. It is possible to define the header outside the canvas app so it can be changed without changing the canvas app. This is a recommended approach.

This canvas component is configured to have a maximum of 20 columns. When a column should not be used:
- set the property "Text" to an empty string ("").
- set the property "Width" to 0.

, for the related header column.

**!! Attention: All 20 columns must be defined.**

### cmp_OnCheck
This custom property contains a required parameter called "cmp_Param_RecordID" which contains the unique ID of the checked details list item (Record ID).

### cmp_OnHeaderSelect
This custom property contains a required parameter called "cmp_Param_Column" which contains the text of the column clicked on.

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_RecordID" which contains the unique ID of the details list item clicked on (Record ID).

### cmp_OnUncheck
This custom property contains a required parameter called "cmp_Param_RecordID" which contains the unique ID of the unchecked details list item (Record ID).

### cmp_TextStyling
This custom property is of data type "Record" and has the following properties:

| Property | Description |
| :--- | :--- |
| Font | The font. |
| FontSize | The font size. |
| HeaderHeight | The height of the header. |
| Padding | The padding. |
| TextBlockHeight | The height of the text block. |
