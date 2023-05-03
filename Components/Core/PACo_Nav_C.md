# PACo_Nav_C.md

This canvas component is meant to be used for a horizontal navigation.

![image](https://user-images.githubusercontent.com/35654198/235981084-9e19c40d-74f4-4f1a-bdb0-fd2b93e4e88a.png)

This is a responsive canvas component.

Clicking on a navigation item navigates to antoher screen. An icon is required.

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Height | Number | The height of the navigation. | 100 |
| cmp_Nav | Table | The navigation items. | *See the documention on navigation menu items below.* |
| cmp_Theme | Record | The theme to use. | *See the documention on theming.* |

### Navigation menu items
A navigation item has the following properties:

| Property | Description |
| :--- | :--- |
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
