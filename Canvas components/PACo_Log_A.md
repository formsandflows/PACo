# PACo_Log_A

This documentation page is related to version: 3.0.0

![image](https://github.com/formsandflows/PACo/assets/35654198/0542a1cf-bef8-428c-9085-09b8ac95d90f)

## Custom properties
| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Add | Action | | Boolean | Add a log item to the collection. | See documentation about cmp_Log below. |
| cmp_HasImages | Data | Input | Boolean | If images are shown in the log or not. | |
| cmp_Log | Data | Output | Table | All log items. | See documentation on cmp_Log below. |
| cmp_LogShown | Data | Output | Table | The log items shown. | See documentation on cmp_Log below. |
| cmp_OnSelect | Event | | Boolean | When a log item is clicked on. | |
| cmp_Reset | Action | | Boolean | Reset the collection with log items. | See documentation on cmp_Log below. |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention on cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Update | Action | | Boolean | Update a log item in the collection. | See documentation on cmp_Log below. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Log
There are 2 collections inside the canvas component:
- coll_Log
- coll_LogShown

This setup allows for the setup to have a collection with all log item and also a collection which is used to display the log items. In the first collection, records can only be added. In the second collectione, records can also be updated.

The custom properties "cmp_Add" and "cmp_Update" have the following parameters:

| Property | Description |
| :--- | :--- |
| cmp_Param_ID | An unique ID of the log item. |
| cmp_Param_Text | A short description. |
| cmp_Param_Account | The account used to run the canvas app. |
| cmp_Param_Clickable | If the log item is clickable or not. |
| cmp_Param_Image | A svg definition for the image. Leave it empty if you do not want to show an image. |
| cmp_Param_ImagePadding | The padding of the image. |
| cmp_Param_Memo | A more extensive description. |
| cmp_Param_User | The selected user. |

All properties except "ID" can be updated with the custom property "cmp_Update" using the ID of a log item. If a value must not be overwriten, it must be set to blank.

If an log item is clickable, a marker is shown before the text.

Having both cmp_Param_Account and cmp_Param_User allows for the situation where the person using the canvas apps has the option to act on behalf of someone else.

Both collections also contain the following additional property:

| Property | Description |
| :--- | :--- |
| DateTime | The date and time when the item was added/updated. |

The collections can be reset with the custom property "cmp_Reset".

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_ID" which contains the ID of the log item clicked on.

### cmp_TextStyling
This custom property is of data type "Record" and has the following properties:

| Property | Description |
| :--- | :--- |
| Align | The horizontal alignment. |
| Color | The color. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| Padding | The padding. |
| TextBlockHeight | The height of text block. |
| VerticalAlign | The vertical alignment. |
