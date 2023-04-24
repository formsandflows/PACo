# PACo_Nav_B

This canvas component is meant to be used for a navigation menu.

[[ IMAGE ]]

A navigation menu navigates between screens.

This component support showing icons, not or both. For the last case, setting alignment is added too.

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Nav | Table | The navigation menu items. | *See the documention on navigation menu items below.* |
| cmp_Theme | Record | The theme to use. | *See the documention on theming.* |
| cmp_Visualization | Text | The visualization to use. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | The color of the visualization. | #0078d4 |

### Navigation menu items
A navigation menu item has the following properties:

| Property | Description |
| :--- | :--- |
| AlignWithImage | Used when not having an icon (image) and to allign the text with navigation menu items who do have an icon. |
| Disabled | Used to disable the navigation menu item. |
| ID | The unique number of the navigation menu item used in the behavior property "cmp_OnSelect". |
| Image | A svg definition to be used as an icon for a non-selected navigation menu item. |
| ImageSelected | A svg definition to be used as an icon for a selected navigation menu item. |
| Order | The order of the item in the navigation menu. |
| Screen | The screen object to navigate to. |
| Text | The text to display. |

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the property "OnSelect" of a navigation menu item. It contains a required parameter (cmp_Param_NavID) which contains the ID of the navigation menu item clicked on. |
