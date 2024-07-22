# PACo_HeaderLanguagesMenu_A

This documentation page is related to version: 3.0.0 and later

Related video page: https://www.formsandflows.nl/paco/videos/paco_headerlanguagesmenu_a/

![image](https://github.com/formsandflows/PACo/assets/35654198/e1a6926c-91d4-4b27-b6bf-aec8cf89c56f)

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_BackgroundColor | Data | Input | Text | The color of the background. | |
| cmp_DividerColor | Data | Input | Text | The color of the divider. | |
| cmp_Languages | Data | Input | Table | The languages menu items. | See the documention about cmp_Languages below. |
| cmp_OnSelect | Event | | Boolean | The event fired when a languages menu item is clicked on. | See the documention about cmp_OnSelect below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Languages
A languages menu item has the following properties:

| Property | Description |
| :--- | :--- |
| ID | The unique ID (text) of the languages menu item used in the custom property "cmp_OnSelect". |
| Image| A svg definition for the image. |
| ImagePadding | The padding of the image. |
| Order | The order of the languages menu item. |

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_LanguageID" which contains the ID of the languages menu item clicked on.
