# PACo_Nav_B

This canvas component is meant to be used for a navigation.

![image](https://user-images.githubusercontent.com/35654198/235980799-970ab7a7-b4e5-4b4f-9270-fdead5e0ad97.png)

Clicking on a navigation item navigates to antoher screen.

This component support showing icons, not or both. For the last case, setting the alignment is added as an option too.

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Nav | Table | The navigation items. | *See the documention on navigation items below.* |
| cmp_Theme | Record | The theme to use. | *See the documention on theming.* |
| cmp_Visualization | Text | The visualization to use. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | The color of the visualization. | #0078d4 |

### Navigation menu items
A navigation item has the following properties:

| Property | Description |
| :--- | :--- |
| AlignWithImage | Used when not having an icon (image) and to allign the text with navigation items who do have an icon. |
| Disabled | Used to disable the navigation item. |
| ID | The unique number of the navigation item used in the behavior property "cmp_OnSelect". |
| Image | A svg definition to be used as an icon for a non-selected navigation item. |
| ImageSelected | A svg definition to be used as an icon for a selected navigation item. |
| Order | The order of the item in the navigation. |
| Screen | The screen object to navigate to. |
| Text | The text to display. |

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the property "OnSelect" of a navigation item (the related icon). It contains a required parameter (cmp_Param_NavID) which contains the ID of the navigation item clicked on. |
