# PACo_Nav_B

This documentation page is related to version: 3.2.0

Related video page: https://www.formsandflows.nl/paco/videos/paco_nav_b/

![image](https://github.com/formsandflows/PACo/assets/35654198/9e2f88a9-1f5b-4e02-b5dd-c584a3e06f77)

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_BackgroundColor | Data | Input | Text | The color of the background. | |
| cmp_DividerColor | Data | Input | Text | The color of the divider. | |
| cmp_Nav | Data | Input | Table | The navigation items. | See the documention about cmp_Nav below. |
| cmp_OnSelect | Event | | None | The event fired when a navigation item is clicked on.  | See the documention about cmp_OnSelect below. |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme to use. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization to use. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Nav
A navigation item has the following properties:

| Property | Description |
| :--- | :--- |
| AlignWithImage | Used when not having an image in the navigation at all (false) or to allign the text with when having an image in the navigation (true). |
| Disabled | Used to disable the navigation item. |
| ID | An unique number of the navigation item used in the custom property "cmp_OnSelect". |
| Image | A svg definition for the image for a non-selected navigation item and when not disabled. |
| ImageDisabled | A svg definition for the image for a non-selected navigation item and when disabled. |
| ImagePadding | The padding of the image. |
| ImageSelected | A svg definition for the image for a selected navigation item. |
| Order | The order of the item in the navigation. |
| Screen | The screen to navigate to. |
| Text | The text. |

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_NavID" which contains the ID of the navigation item clicked on.

### cmp_TextStyling
This custom property has the following properties:

| Property | Description |
| :--- | :--- |
| Color | The color. |
| ColorDisabled | The color when the navigation item is disabled. |
| ColorSelected | The color when the navigation item is selected. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| TextBlockHeight | The height of the text block. |
