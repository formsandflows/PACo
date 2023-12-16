# cmp_Header_A

This canvas component is meant to be used for a header.

![PACo_Header](https://user-images.githubusercontent.com/35654198/197222197-cffad482-52b7-483d-9d43-6bdc93954b28.png)

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Back | Boolean | This property determines if the back icon is shown. | true |
| cmp_Help | Boolean | This property determines if the help icon is shown. | true |
| cmp_Settings | Boolean | This property determines if the settings icon is shown. | true |
| cmp_SettingsSelected | Boolean | This property is used to show the proper icon for the settings menu. | true |
| cmp_Theme | Record | This property contains the theme to use for the header. | *See the documention on theming.* |
| cmp_Title | Text | This property contains the title of the header. | Reload |
| cmp_Visualization | Text | This property contains the visualization. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | This property contains the color to use in the visualization. | #0078d4 |

### Back icon
This icon is used in setting screens to go back to the screen from where the settings screen was called.

### Help icon
This icon is used to redirect an user to a location where (s)he can find more information.

### Settings icon
This icon is used to show a settings menu. A settings component, like cmp_Settings_A, can be used to display a settings menu.

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnBackSelect | This property is related to the property "OnSelect" of the back icon. |
| cmp_OnHelpSelect | This property is related to the property "OnSelect" of the help icon. |
| cmp_OnSettingsSelect | This property is related to the property "OnSelect" of the settings icon. |
