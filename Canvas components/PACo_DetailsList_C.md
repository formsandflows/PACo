# PACo_DetailsList_C

This documentation page is related to version: 3.2.0

Related video page: https://www.formsandflows.nl/paco/videos/paco_detailslist_c/

![image](https://github.com/formsandflows/PACo/assets/35654198/f942a4d6-7f2b-4a41-9249-2da47aae3ba3)

Per details list item, up to 3 fields can be shown:
* Title.
* Subtitle.
* Body.
All fields are based on a label control. The subtitle is displayed in italics. The property "Overflow" of the body is: Scroll

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_BackgroundColor | Data | Input | Text | The color of the background. | |
| cmp_CheckboxColor | Data | Input | Text | The color of the checkbox. | |
| cmp_DetailsList | Data | Input | Table | The details list items. | See the documention about cmp_DetailsList below. |
| cmp_DividerColor | Data | Input | Text | The color of the divider. | |
| cmp_OnCheck | Event | | None | The event fired when the item checkbox is clicked on and the checkbox is unchecked. | See the documention about cmp_OnCheck below. |
| cmp_OnSelect | Event | | None | The event fired when a details list item is clicked on. | See the documention on cmp_OnSelect below. |
| cmp_OnUncheck | Event | | None | The event fired when the item checkbox is clicked on and the checkbox is checked. | See the documention about cmp_OnUncheck below. |
| cmp_ShowCheckbox | Data | Input | Boolean | To show the checkbox for details list items or not. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention on about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_DetailsList
To have a more consistent naming with the other details list components in PACo, several properties contain the text "Column" which can be read as "Field".

The properties have "Small" in their naming so 1 collection for the details list items can be used by an instance of this canvas component as well as an instance of a details list canvas component when the screen has more width (PACo_DetailsList_A or PACo_DetailsList_B). With this setup, the first 3 columns in this details list can also differ from the first 3 columns when the screen has more width.

For each details list item, the following properties must be available:
- Column1SmallColor
- Column1SmallColorSelected
- Column1SmallFontSize
- Column1SmallFontWeight
- Column1SmallText
- Column2SmallColor
- Column2SmallColorSelected
- Column2SmallFontSize
- Column2SmallFontWeight
- Column2SmallText
- Column3SmallColor
- Column3SmallColorSelected
- Column3SmallFontSize
- Column3SmallFontWeight
- Column3SmallText
- SmallFill
- SmallFillSelected

Only the use of a collection which contains the details list items is supported! Dataverse tables, SharePoint lists, ... can thus not directly be connected to the property "cmp_DetailsList".

The collection which contains the details list items must have the additional required properties:

| Property | Description |
| :--- | :--- |
| RecordID | An unique ID of the details list item. This property is of type "Text".  |
| Selected | This property must be set when checking/unchecking a details list item. This property is of type "Boolean". |

### cmp_OnCheck
This custom property contains a required parameter called "cmp_Param_RecordID" which contains the unique ID of the selected item (Record ID).

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_RecordID" which contains the unique ID of the selected details list item (Record ID).

### cmp_OnUncheck
This custom property contains a required parameter called "cmp_Param_RecordID" which contains the unique ID of the selected item (Record ID).

### cmp_TextStyling
This custom property has the following properties:

| Property | Description |
| :--- | :--- |
| BodyHeight | The height of the body. |
| Font | The font. |
| TextBlockHeight | The height of the text block of the title and of the subtitle. |

All details list items have the same height and is defined as 2 times TextBlockHeight plus BodyHeight.

| Situation | Description |
| :--- | :--- |
| Title and Subtitle | BodyHeight = 0 |
| Title and Body | BodyHeight = Required body height minus TextBlockHeight |
| Title, Subtitle and Body | BodyHeight = Required body height |
