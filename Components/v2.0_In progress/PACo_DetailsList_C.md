# PACo_DetailsList_A

This canvas component is meant to be used for a details list when the screen has a snall width.

Per item, up to 3 fields can be shown:
* Title which is based on a label control.
* Subtitle which is based on a label control.
* HTML which is based on a html control.

[[IMAGE]]

## **Input properties**

### Details list items

To have a more consistant naming, several properties contain the text "Column" which can be read a "Field".

For each column, the following properties must be available:
- Column1Color
- Column1FontWeight
- Column1Text
- Column2Color
- Column2FontWeight
- Column2Text
- Column3Text

The collection to display the items has an additional required property:

| Property | Description |
| :--- | :--- |
| RecordID | The unique ID of the item. This property is of type "Text".  |

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnCheck | This property is related to the property "OnCheck" of the checkbox of an item. It contains a required parameter (cmp_Param_RecordID) which contains the unique ID of the selected item. |
| cmp_OnUncheck | This property is related to the property "OnUncheck" of the checkbox of an item. It contains a required parameter (cmp_Param_RecordID) which contains the unique ID of the selected item. |
