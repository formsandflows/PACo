# PACo_Header_A

This canvas component is meant to be used for a header.

[[ IMAGE ]]

The back and navigation menu icon share the same location and thus cannot be used simultaneously.

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Back | Boolean | To show the back icon. | true |
| cmp_Help | Boolean | To show the help icon. | true |
| cmp_NavMenu | Boolean | To show the navigation menu. | true |
| cmp_NavMenuSelected | Boolean | The show the correct icon for the navigation menu. | true |
| cmp_SettingsMenu | Boolean | To show the settings menu. | true |
| cmp_SettingsMenuSelected | Boolean | The show the correct icon for the settings menu. | true |
| cmp_Theme | Record | The theme to use. | *See the documention on theming.* |
| cmp_Title | Text | The text to show in the header. | Home Screen |
| cmp_Visualization | Text | The visualization to use. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | The color of the visualization. | #0078d4 |

### Back icon
This icon is used in setting screens to go back to the screen from where the settings screen was called.

### Help icon
This icon is used to redirect an user to a location where (s)he can find more information.

### Navigation menu icon
This icon is used to show a navigation menu. A navigation menu component (like PACo_Nav_B) can be used to display a navigation menu.

The navigation menu icon is meant to be used for situations when a navigation menu cannot be shown due to a lack of space. For instance for mobile app development.

### Settings menu icon
This icon is used to show a settings menu. A settings menu component (like PACo_Settings_A) can be used to display a settings menu.

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnBackSelect | This property is related to the property "OnSelect" of the back icon. |
| cmp_OnHelpSelect | This property is related to the property "OnSelect" of the help icon. |
| cmp_OnNavMenuSelect | This property is related to the property "OnSelect" of the navigation menu icon. |
| cmp_OnSettingsMenuSelect | This property is related to the property "OnSelect" of the settings menu icon. |
