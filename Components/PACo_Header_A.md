# PACo_Header_A

!! The current active version is version 2.2. This file is already here because on version 3.0 (or better: release 3.0) is currently actively worked on.

This page is related to version: 3.0

![image](https://user-images.githubusercontent.com/35654198/235980652-ab1d1a83-c6f3-4f66-861f-3911ff817749.png)

This is a responsive canvas component.

You can use the canvas app "PACo Examples" for a better understanding of, and to experiment with, this canvas component.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_Images | Data | Input | Table | Properties of the images. | See the documention on cmp_Images below. |
| cmp_NavSelected |  Data | Input | Boolean | To show the correct image for the navigation. | |
| cmp_OnBackSelect | Event | | Boolean | When the back image is clicked on. | |
| cmp_OnHelpSelect | Event | |  Boolean | When the help image is clicked on. | |
| cmp_OnNavSelect | Event | | Boolean | When the navigation image is clicked on. | |
| cmp_OnSettingsMenuSelect | Event | | Boolean | When the settings menu image is clicked on. | |
| cmp_SettingsMenuSelected | Data | Input | Boolean | The show the correct icon for the settings menu. | |
| cmp_ShowBack | Data | Input | Boolean | To show the back image or not. | See the documention on cmp_ShowBack below. |
| cmp_ShowHelp | Data | Input | Boolean | To show the help image or not. |See the documention on cmp_ShowHelp below. |
| cmp_ShowNav | Data | Input | Boolean | To show the navigation image or not. |See the documention on cmp_ShowNav below. |
| cmp_ShowSettingsMenu | Data | Input | Boolean | To show the settings menu image or not. |See the documention on cmp_ShowSettingsMenu below. |
| cmp_Text | Data | Input | Text | The text. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention on cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Images
This custom property is of data type "Table" and a record has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID for the image. |
| Image | A svg definition for the image. |
| ImagePadding | The padding of the image. |

#### cmp_ShowBack
The idea behind this image is that it is used on setting screens to go back to the screen where the settings screen was called from.

The back image and the navigation image share the same location and thus cannot be used simultaneously.

#### cmp_ShowHelp
This image is used to redirect an user to a location where (s)he can find more information.

#### cmp_ShowNav
This image is used to show a navigation. A navigation canvas component like "PACo_Nav_B" can be used to display a navigation.

The navigation image is meant to be used for situations when a navigation cannot be shown by default due to a lack of space. For instance for mobile app development.

#### cmp_ShowSettingsMenu
This image is used to show a settings menu. A settings menu component like "PACo_SettingsMenu_A" can be used to display a settings menu.

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
| VerticalAlign | The vertical alignment. |
