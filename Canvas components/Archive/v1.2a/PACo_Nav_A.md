# PACo_Nav_A

This canvas component is meant to be used for a navigation menu.

![PACo_Nav](https://user-images.githubusercontent.com/35654198/197222505-7e7f42d7-9014-4471-a93a-c37c3f97a3e4.png)

A navigation menu navigates between screens.

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Nav | Table | This property contains the menu items. | *See the documention on menu items below.* |
| cmp_Theme | Record | This property contains the theme to use for the navigation menu. | *See the documention on theming.* |
| cmp_Visualization | Text | This property contains the visualization. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | This property contains the color to use in the visualization. | #0078d4 |

### Menu items
A menu item has the following properties:

| Property | Description |
| :--- | :--- |
| ID | The unique number of the menu item used in the behavior property "cmp_OnSelect". |
| Order | The order of the menu item in the navigation menu. |
| Screen | The screen object to navigate to. |
| Text | The text to display. |

Example:

`Table({ID:1, Order:10, Screen:'Home Screen', Text:"Home Screen"}, {ID:2, Order:20, Screen:'Second Screen', Text:"Second screen"})`

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the property "OnSelect" of a menu item. It contains a required parameter (cmp_Param_NavID) which contains the ID of the menu item clicked on. |
