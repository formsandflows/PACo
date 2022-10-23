# cmp_Details_A

This canvas component is meant to be used for a details list.

![PACo_DetailsList](https://user-images.githubusercontent.com/35654198/197223074-306fa0fb-965e-43f3-8f03-c0aedc500a55.png)

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_DetailsList | Table | This property contains the details list items. | *See the documention on details list items below.* |
| cmp_ElevationColor | Text | This property contains the color to use in the elevation of the details list. | #0078d4 |
| cmp_Header | Record | This property contains the details list header | *See the documention on details list header below.* |
| cmp_SortingColumn | Text | This property is used to determine where to show the sorting icon | Field1 |
| cmp_SortingDirection | Text | This property is used to show the sorting icon on a header column | Ascending |
| cmp_ResetCheckboxHeader | Boolean | This property is used to reset the checkbox in the header of the details list. | true |
| cmp_Theme | Record | This property contains the theme to use for the details list. | *See the documention on themes.* |

### Details list header

### Details list items

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnCheck | This property is related to the OnCheck property of the checkbox in the gallery (cb_DetailsList_A_Gall). It contains a required parameter (cmp_Param_RecordID) which contains the unique ID of the selected item (record). |
| cmp_OnCheckAll | This property is related to the OnCheck property of the checkbox in the header (cb_DetailsList_A_Header). |
| cmp_OnHeaderSelect | This property is related to the OnSelect property of all header icons. It contains a required parameter (cmp_Param_Column) which contains the name of the column clicked on. |
| cmp_OnSelect | This property is related to the OnSelect property of all labels in the gallery (lbl_DetailsList_A_Gall_#). It contains a required parameter (cmp_Param_RecordID) which contains the unique ID of the selected item (record). |
| cmp_OnUncheck | This property is related to the OnUncheck property of the checkbox in the gallery (cb_DetailsList_A_Gall). It contains a required parameter (cmp_Param_RecordID) which contains the unique ID of the selected item (record). |
| cmp_OnUncheckAll | This property is related to the OnCheck property of the checkbox in the header (cb_DetailsList_A_Header). |
