# PACo_DetailsList_A

This canvas component is meant to be used for a details list.

![image](https://user-images.githubusercontent.com/35654198/235978809-ca5d0c95-df32-4ea2-b304-88520dbdd83f.png)

This is a responsive canvas component. A horizontal scroll can appear when the width of the details list is more than fits on the screen.

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_DetailsList | Table | The details list items. | *See the documention on details list items below.* |
| cmp_Header | Record | The details list header. Every header column has its own subrecord. | *See the documention on details list header below.* |
| cmp_ResetCheckbox | Boolean | To reset the checkbox of all items in the details list component. | true |
| cmp_ResetCheckboxHeader | Boolean | To reset the checkbox in the header. | true |
| cmp_ShowCheckbox | Boolean | To show the checkbox at the details list items or not. | true |
| cmp_ShowCheckboxHeader | Boolean | To show the checkbox in the header or not. | true |
| cmp_SortingColumn | Text | The column to sort on. | Column1Text |
| cmp_SortingDirection | Text | The sorting direction. | Ascending |
| cmp_Theme | Record | The theme to use. | *See the documention on theming.* |
| cmp_Visualization | Text | The visualization to use. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | The color of the visualization. | #0078d4 |

### Details list header

A header column has the following properties:

| Property | Description |
| :--- | :--- |
| Sortable | This determines if the related header column can be used for sorting. |
| Text | The text to show in the related label control. |
| Width | The width of the related label control. |

The width of a header can thus be configured but is fixed when using the app. It is possible to define the header outside the canvas app so it can be changed without changing the canvas app. This is a recommended approach.

If the total width of all columns together is larger than the width of the details list component, a horizontal scrollbar is shown.

This component is configured to have a maximum of 20 columns. When a column shoud not be used:

- set the property "Title" to an empty string ("").
- set the property "Width" to 0.

, for the related header column.

**!! Attention: All 20 columns must be defined.**

### Details list items

This component is configured to have a maximum of 20 columns. To be able to display the items, a collection with a pre-defined set of required(!) properties must be used. This was needed to make this canvas component a generic canvas component.

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

Only the use of a collection which contains the details list items is supported (read: configured/tested)! Dataverse tables, SharePoint lists, ... can thus not directly be connected to the property "cmp_DetailsList".

The collection to display the details list items must have 2 additional required properties:

| Property | Description |
| :--- | :--- |
| RecordID | The unique ID of the details list item. This property is of type "Text". |
| Selected | This property must be set when checking/unchecking a details list item. This property is of type "Boolean". |

**!! Attention: All 20 columns must be defined.**

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnCheck | This property is related to the property "OnCheck" of the checkbox of a details list item. It contains a required parameter (cmp_Param_RecordID) which contains the unique ID of the selected item (Record ID). |
| cmp_OnCheckAll | This property is related to the property "OnCheck" of the checkbox in the header. |
| cmp_OnHeaderSelect | This property is related to the property "OnSelect" of all header column icons. It contains a required parameter (cmp_Param_Column) which contains the name of the column clicked on. |
| cmp_OnSelect | This property is related to the property "OnSelect" of all items (or more detailed: all label controls in the gallery used to show the items). It contains a required parameter (cmp_Param_RecordID) which contains the unique ID of the selected details list item (Record ID). |
| cmp_OnUncheck | This property is related to the property "OnUncheck" of the checkbox of a details list item. It contains a required parameter (cmp_Param_RecordID) which contains the unique ID of the selected details list item (Record ID). |
| cmp_OnUncheckAll | This property is related to the property "OnUncheck" of the checkbox in the header. |
