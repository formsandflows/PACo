# PACo_Nav_B

This canvas component is meant to be used for a navigation menu. This component divers from "PACo_Nav_A" in that it can contain also an image.

![PACo_Nav_B](https://user-images.githubusercontent.com/35654198/221430546-5e73cac4-4d59-4c27-9a1b-e7fd9792d8a2.png)

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
| HasIcon | Used to show the image or not. |
| ID | The unique number of the menu item used in the behavior property "cmp_OnSelect". |
| Image | The image to show. |
| Order | The order of the menu item in the navigation menu. |
| Screen | The screen object to navigate to. |
| Text | The text to display. |

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the property "OnSelect" of a menu item. It contains a required parameter (cmp_Param_NavID) which contains the ID of the menu item clicked on. |
