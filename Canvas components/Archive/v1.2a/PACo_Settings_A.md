# PACo_Settings_A

This canvas component is meant to be used for a settings menu.

![image](https://user-images.githubusercontent.com/35654198/197237104-e6406f0c-81e6-4c46-824f-31b873505c1d.png)

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Menu | Table | This property contains the menu items. | *See the documention on menu items below.* |
| cmp_Theme | Record | This property contains the theme to use for the settings menu. | *See the documention on theming.* |
| cmp_Visualization | Text | This property contains the visualization. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | This property contains the color to use in the visualization. | #0078d4 |
| cmp_Width | Number | This property contains the width of the settings menu. | 400 |

### Menu items

A menu item has the following properties:

| Property | Description |
| :--- | :--- |
| ID | The unique number of the menu item used in the behavior property "cmp_OnSelect". |
| Order | The order of the menu item in the settings menu. |
| Screen | The screen control to navigate to. |
| Text | The text to display. |

Example:

`Table({ID:1, Order:10, Screen:'Theme Screen', Text:"Themes"}, {ID:2, Order:20, Screen:'Language Screen', Text:"Languages"})`

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the property "OnSelect" of a menu item. It contains a required parameter (cmp_Param_SettingsID) which contains the ID of the menu item clicked on. |
