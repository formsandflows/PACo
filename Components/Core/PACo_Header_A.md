# PACo_Header_A

This canvas component is meant to be used for a header.

![image](https://user-images.githubusercontent.com/35654198/235980652-ab1d1a83-c6f3-4f66-861f-3911ff817749.png)

This is a responsive canvas control.

The back and navigation menu icon share the same location and thus cannot be used simultaneously.

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_NavSelected | Boolean | The show the correct icon for the navigation menu. | true |
| cmp_SettingsMenuSelected | Boolean | The show the correct icon for the settings menu. | true |
| cmp_ShowBack | Boolean | To show the back icon or not. | true |
| cmp_ShowHelp | Boolean | To show the help icon or not. | true |
| cmp_ShowNav | Boolean | To show the navigation menu or not. | true |
| cmp_ShowSettingsMenu | Boolean | To show the settings menu or not. | true |
| cmp_Theme | Record | The theme to use. | *See the documention on theming.* |
| cmp_Title | Text | The text to show in the header. | Home Screen |
| cmp_Visualization | Text | The visualization to use. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | The color of the visualization. | #0078d4 |

### Back icon
This icon is used in setting screens to go back to the screen from where the settings screen was called.

### Help icon
This icon is used to redirect an user to a location where (s)he can find more information.

### Navigation icon
This icon is used to show a navigation. A navigation component (like PACo_Nav_B) can be used to display a navigation.

The navigation icon is meant to be used for situations when a navigation cannot be shown due to a lack of space. For instance for mobile app development.

### Settings menu icon
This icon is used to show a settings menu. A settings menu component (like PACo_Settings_A) can be used to display a settings menu.

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnBackSelect | This property is related to the property "OnSelect" of the back icon. |
| cmp_OnHelpSelect | This property is related to the property "OnSelect" of the help icon. |
| cmp_OnNavSelect | This property is related to the property "OnSelect" of the navigation icon. |
| cmp_OnSettingsMenuSelect | This property is related to the property "OnSelect" of the settings menu icon. |
