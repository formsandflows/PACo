# PACo_Nav_C

> [!WARNING]
> This page is a pre-release page. It contains documentation for a future release. Please look in de folder "Archive" for documentation on released versions.

This documentation page is related to version: 3.2.0

Related video page: https://www.formsandflows.nl/paco/videos/paco_nav_c/

![image](https://github.com/formsandflows/PACo/assets/35654198/05316c96-4768-4834-94e1-0d0c1407e240)

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_BackgroundColor | Data | Input | Text | The color of the background. | |
| cmp_DividerColor | Data | Input | Text | The color of the divider. | |
| cmp_OnSelect | Event | | None | The event fired when a navigation item is clicked on. | See the documention about cmp_OnSelect below. |
| cmp_Nav | Data | Input | Table | The navigation items. | See the documention about cmp_Nav below. |
| cmp_PercentageTextHeight | Data | Input | Number | The percentage of the height for the text section. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |

### cmp_Nav
A navigation item has the following properties:

| Property | Description |
| :--- | :--- |
| Disabled | Used to disable the navigation item. |
| ID | An unique number of the navigation item used in the behavior property "cmp_OnSelect". |
| Image | A svg definition for the image for a non-selected navigation item and when not disabled. |
| ImageDisabled | A svg definition for the image for a non-selected navigation item and when disabled. |
| ImagePadding | The padding of the image. |
| ImageSelected | A svg definition for the image for a selected navigation item. |
| Order | The order of the navigation item. |
| Screen | The screen object to navigate to. |
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
| Padding | The padding. |
| VerticalAlign | The vertical alignment. |
