# cmp_DetailsList_A

This canvas component is meant to be used for a details list.

![PACo_DetailsList](https://user-images.githubusercontent.com/35654198/197223074-306fa0fb-965e-43f3-8f03-c0aedc500a55.png)

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_DetailsList | Table | This property contains the details list items. | *See the documention on details list items below.* |
| cmp_Header | Record | This property contains the details list header | *See the documention on details list header below.* |
| cmp_SortingColumn | Text | This property is used to determine where to show the sorting icon | Field1 |
| cmp_SortingDirection | Text | This property is used to show the sorting icon on a header column | Ascending |
| cmp_ResetCheckboxHeader | Boolean | This property is used to reset the checkbox in the header of the details list. | true |
| cmp_Theme | Record | This property contains the theme to use for the details list. | *See the documention on theming.* |
| cmp_Visualization | Text | This property contains the visualization. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | This property contains the color to use in the visualization. | #0078d4 |

### Details list header

A header column has the following properties:

| Property | Description |
| :--- | :--- |
| Sortable | This determines if the related header column can be used for sorting. |
| Title | The title of the related label control. |
| Width | The width of the related label control. |

Example:

`{Title1:"Item type", Width1:240, Sortable1:true, Title2:"Order date", Width2:140, Sortable2:true, ...}`

The width of a header can thus be configured but is fixed when using the app. It is possible to define the header outside the canvas app so it can be changed without chanign the canvas app. This is a recommended approach.

If the total width of the columns or larger than the width of the details list component, a horizontal scrollbar is shown.

This component is set up to have a maximum of 10 columns. When a column shoud not be used:

- The property "Title#" must be set to an empty string ("").
- The property "Width#" must be set to 0.

, where # is the number of the column.

**!! Attention: All 16 columns must be defined.**

### Details list items

This component is set up to have a maximum of 16 columns per item and each column has a fixed internal name: Field1, Field2, ... This was needed to make this canvas component a generic canvas component. These properties are of type "Text".

Besides the fixed internal name, each column has 4 extra properties (type "Text"):
- Field#Color
- Field#ColorSelected
- Field#ColorBackground
- Field#ColorBackgroundSelected
, where # is the number of the column. These properties hold color values (Example: #00ff00) and can be used to format a column.

Only the use of collections for the items is supported (read: configured/tested)! Dataverse tables, SharePoint lists, ... can thus not directly be connected to the property "cmp_DetailsList".

The columns that are defined in the header (cmp_Header) must be available in the collection that is used for the items.

There are 2 additional required properties:

| Property | Description |
| :--- | :--- |
| RecordID | The unique ID of the item. This property is of type "Text".  |
| Selected | This property is used when checking/unchecking an item. This property is of type "Boolean". |

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnCheck | This property is related to the property "OnCheck" of the checkbox of an item. It contains a required parameter (cmp_Param_RecordID) which contains the unique ID of the selected item (record). |
| cmp_OnCheckAll | This property is related to the property "OnCheck" of the checkbox in the header. |
| cmp_OnHeaderSelect | This property is related to the property "OnSelect" of all header icons. It contains a required parameter (cmp_Param_Column) which contains the name of the column clicked on. |
| cmp_OnSelect | This property is related to the property "OnSelect" of all items (or more detailed: all label controls in the gallery used to show the items). It contains a required parameter (cmp_Param_RecordID) which contains the unique ID of the selected item (record). |
| cmp_OnUncheck | This property is related to the property "OnUncheck" of the checkbox of an item. It contains a required parameter (cmp_Param_RecordID) which contains the unique ID of the selected item (record). |
| cmp_OnUncheckAll | This property is related to the property "OnUncheck" of the checkbox in the header. |
