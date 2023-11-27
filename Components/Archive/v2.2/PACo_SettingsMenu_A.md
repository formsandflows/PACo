# PACo_SettingsMenu_A

This page is related to version: 2.2

This canvas component is meant to be used for a settings menu.

![image](https://user-images.githubusercontent.com/35654198/235982163-5c2ef64a-9f0f-4e69-8c3a-5003116f13f3.png)

A settings menu is activated using the setting menu icon in the header. Selecting a settings menu item navigates to another screen.

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Menu | Table | The settings menu items. | *See the documention on settings menu items below.* |
| cmp_Theme | Record | The theme to use. | *See the documention on theming.* |
| cmp_Visualization | Text | The visualization to use. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | The color of the visualization. | #0078d4 |
| cmp_Width | Number | The width of the settings menu. | 400 |

### Setings menu items

A settings menu item has the following properties:

| Property | Description |
| :--- | :--- |
| Disabled | If the menu item is disabled or not. |
| ID | The unique number of the settings menu item used in the behavior property "cmp_OnSelect". |
| Order | The order of the item in the settings menu. |
| Screen | The screen control to navigate to. |
| Text | The text to display. |

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the property "OnSelect" of the icon control used to display a settings menu item. It contains a required parameter (cmp_Param_SettingsID) which contains the ID of the settings menu item clicked on. |
