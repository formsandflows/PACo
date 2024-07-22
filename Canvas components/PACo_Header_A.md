# PACo_Header_A

> [!WARNING]
> This page is a pre-release page. It contains documentation for a future release. Please look in de folder "Archive" for documentation on released versions.

This documentation page is related to version: 3.2.0

Related video page: https://www.formsandflows.nl/paco/videos/paco_header_a/

![image](https://github.com/formsandflows/PACo/assets/35654198/ef050772-7f67-484c-b6bf-dee0aaae5bdf)

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_BackgroundColor | Data | Input | Text | The color of the background. | |
| cmp_Images | Data | Input | Table | Properties of the images. | See the documention about cmp_Images below. |
| cmp_LanguagesMenuImage | Data | Input | Record | A svg definition for the languages menu image. | See the documention about cmp_LanguagesMenuImage below. |
| cmp_LanguagesMenuPropertyX | Data | Output | Number | The X value for the languages menu. | |
| cmp_Logo | Data | Input | Record | The logo. | See the documention about cmp_Logo below. |
| cmp_OnBackSelect | None | | Boolean | The event fired when the back image is clicked on. | |
| cmp_OnHelpSelect | None | |  Boolean | The event fired when the help image is clicked on. | |
| cmp_OnLanguagesMenuSelect | None | | Boolean | The event fired when the languages menu image is clicked on. | |
| cmp_OnLogoSelect | None | | Boolean | The event fired when the logo image is clicked on. | |
| cmp_OnNavSelect | None | | Boolean | The event fired when the navigation image is clicked on. | |
| cmp_OnSettingsMenuSelect | None | | Boolean | The event fired when the settings menu image is clicked on. | |
| cmp_ShowBack | Data | Input | Boolean | To show the back image or not. | See the documention about cmp_ShowBack below. |
| cmp_ShowHelp | Data | Input | Boolean | To show the help image or not. | See the documention about cmp_ShowHelp below. |
| cmp_ShowLanguagesMenu | Data | Input | Boolean | To show the languages menu image or not. | See the documention about cmp_ShowLanguagesMenu below. |
| cmp_ShowLogo | Data | Input | Boolean | To show the logo image or not. | See the documention about cmp_ShowLogo below. |
| cmp_ShowNav | Data | Input | Boolean | To show the navigation image or not. | See the documention about cmp_ShowNav below. |
| cmp_ShowSettingsMenu | Data | Input | Boolean | To show the settings menu image or not. | See the documention about cmp_ShowSettingsMenu below. |
| cmp_Text | Data | Input | Text | The text. | |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Images
This custom property is of data type "Table" and a record has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID for the image. |
| Image | A svg definition for the image. |
| ImagePadding | The padding of the image. |

### cmp_LanguagesMenuImage
This custom property is of data type "Record" and has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID of the language. |
| Image | A svg definition for the image. |
| ImagePadding | The padding of the image. |

### cmp_Logo
This custom property is of data type "Record" and has the following properties:

| Property | Description |
| :--- | :--- |
| Clickable | If the logo is clickable ir not. |
| Height | The original height of the svg image. |
| Image | A svg definition for the image. |
| ImagePaddingHeight | The padding at the top and bottom. |
| ImagePaddingWidth | The padding at the left and right. |
| Width | The original width of the svg image. |

### cmp_ShowBack
This custom property is used to show the back image on setting screens to go back to the screen where the settings screen was called from when the related image is clicked on (cmp_OnBackSelect). This is normally the home screen.

The back image and the navigation image share the same location and thus cannot be used simultaneously!

The back image is not shown in the image above.

### cmp_ShowHelp
This custom property is used to show the help image which allows to redirect an user to a location where (s)he can find more information when the image is clicked on (cmp_OnHelpSelect).

### cmp_ShowLanguagesMenu
This custom property is used to show a languages menu image. A languages menu component like "PACo_LanguagesMenu_A" can be used to display a languages menu when the image is clicked on (cmp_OnLanguagesMenuSelect).

### cmp_ShowLogo
This custom property is used to show the logo. A logo can be clickable or not. When it is clickable and clicked on, the cmp_OnLogoSelect event is triggered.

### cmp_ShowNav
This custom property is used to show a navigation image. A navigation canvas component like "PACo_Nav_B" can be used to display a navigation when the image is clicked on (cmp_OnNavSelect).

The navigation image is meant to be used for situations when a navigation cannot be shown due to a lack of space. For instance for mobile app development.

### cmp_ShowSettingsMenu
This custom property is used to show a settings menu image. A settings menu component like "PACo_SettingsMenu_A" can be used to display a settings menu when the image is clicked on (cmp_OnSettingsMenuSelect).

### cmp_TextStyling
This custom property has the following properties:

| Property | Description |
| :--- | :--- |
| Align | The horizontal alignment. |
| Color | The color. |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| Padding | The padding. |
| VerticalAlign | The vertical alignment. |
