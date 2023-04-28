# PACo_CommandBarMenu_A

This canvas component is meant to be used for a menu for a command bar.

[[ IMAGE ]]

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Menu | Table | The command bar menu items. | *See the documention on command bar menu items below.* |
| cmp_Theme | Record | The theme to use. | *See the documention on theming.* |
| cmp_Visualization | Text | The visualization to use. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | The color of the visualization. | #0078d4 |

### Command bar menu items
A command bar menu item has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID (number) of the command bar menu item. |
| SelectedItems | When to show the command bar item. *See the documention on the component "cmp_CommandBar_A".* |
| Text | The text to display in the related label control. |
| Title | The internal name of the command bar menu item. This is needed to support multilingual canvas apps. |

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the property "OnSelect" of the icon control in the gallery used for the command bar menu. It contains a required parameter (cmp_Param_CommandID) which contains the  ID of the command bar menu item clicked on. |
