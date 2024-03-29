# PACo_CommandBarMenu_A

This page is related to version: 2.2

This canvas component is meant to be used for a command bar menu.

![image](https://user-images.githubusercontent.com/35654198/235977451-6a35b6da-012f-48ba-bbd5-719c261c28c3.png)

This is a responsive canvas component but usually a lot of width is needed for this canvas component. To still use this canvas component when the screen has a small width, you can place this canvas component in a responsive horizontal container to get a horizontal scroll bar. See the canvas component "PACo_DetailsList_B" for an example.

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_ImagePadding | Number | The padding of the icons. | 10 |
| cmp_Menu | Table | The command bar menu items. | *See the documention on command bar menu items below.* |
| cmp_Theme | Record | The theme to use. | *See the documention on theming.* |
| cmp_Visualization | Text | The visualization to use. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | The color of the visualization. | #0078d4 |

### Command bar menu items
A command bar menu item has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID (number) of the command bar menu item. |
| Image| A svg definition to be used as an icon. |
| Text | The text to display in the related label control. |
| Title | The internal name of the command bar menu item. This is needed to support multilingual canvas apps. |

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the property "OnSelect" of the icon control in the gallery used for the command bar menu. It contains a required parameter (cmp_Param_CommandID) which contains the  ID of the command bar menu item clicked on. |
