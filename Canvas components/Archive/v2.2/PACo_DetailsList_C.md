# PACo_DetailsList_C

This page is related to version: 2.2

This canvas component is meant to be used for a details list when the screen has a small width.

![image](https://user-images.githubusercontent.com/35654198/235979572-89783b98-c265-44c7-b2ef-e3f8158662b7.png)

Per item, up to 3 fields can be shown:
* Title which is based on a label control.
* Subtitle which is based on a label control.
* HTML which is based on a html control.

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_BodyHeight | Number | The height of the body control. | 80 |
| cmp_DetailsList | Table | The details list items. | *See the documention on details list items below.* |
| cmp_ResetCheckbox | Boolean | To reset the checkbox of all items in the details list component. | true |
| cmp_ShowCheckbox | Boolean | To show the checkbox at the details list items or not. | true |
| cmp_Theme | Record | The theme to use. | *See the documention on theming.* |
| cmp_Visualization | Text | The visualization to use. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | The color of the visualization. | #0078d4 |

### Details list items

To have a more consistent naming with the other details list components in PACo-Core, several properties contain the text "Column" which can be read a "Field".

The properties have "Small" in their naming so 1 collection can be used to be used by this canvas component as well as a canvas component to used when the screen has more width. With this setup, the first 3 columns can differ instead of having to be the same.

For each details list item, the following properties must be available:
- Column1SmallColor
- Column1SmallFontWeight
- Column1SmallText
- Column2SmallColor
- Column2SmallFontWeight
- Column2SmallText
- Column3SmallText
- SmallFill
- SmallFillSelected

Only the use of a collection which contains the details list items is supported (read: configured/tested)! Dataverse tables, SharePoint lists, ... can thus not directly be connected to the property "cmp_DetailsList".

The collection to display the details list items must have the additional required property:

| Property | Description |
| :--- | :--- |
| RecordID | The unique ID of the item. This property is of type "Text".  |
| Selected | This property must be set when checking/unchecking a details list item. This property is of type "Boolean". |

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnCheck | This property is related to the property "OnCheck" of the checkbox of a details list item. It contains a required parameter (cmp_Param_RecordID) which contains the unique ID of the selected item (Record ID). |
| cmp_OnUncheck | This property is related to the property "OnUncheck" of the checkbox of a details list item. It contains a required parameter (cmp_Param_RecordID) which contains the unique ID of the selected item (Record ID). |
