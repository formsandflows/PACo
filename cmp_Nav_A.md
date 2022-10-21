This canvas component is meant to be used for a navigation menu.

![PACo_Nav](https://user-images.githubusercontent.com/35654198/197222505-7e7f42d7-9014-4471-a93a-c37c3f97a3e4.png)

A navigation menu navigates between screen.

## **Input properties**

| Property | Type | Description | Example |
| - | - | - | - |
| cmp_ElevationColor | Text | This property contains the color to use in the elevation of the navigation menu. | #0078d4 |
| cmp_Nav | Table | This property contains the menu items. | *See the documention on menu items below.* |
| cmp_Theme | Record | This property contains the theme to use for the navigation menu. | *See the documention on themes.* |

### menu items
A menu item has the following properties:

| Property | Description |
| - | - |
| ID | The unique number of the menu item used in the behavior property "cmp_OnSelect" |
| Title | The title of the menu item |
| Screen | The screen control to navigate to |
| Order | The order of the menu item in the navigation menu |

Example:

Table({ID:1, Title:"Home Screen", Screen:App.ActiveScreen, Order:10}, {ID:2, Title:"Second Screen", Screen:App.ActiveScreen, Order:20})

### Redirect Screen
The companion app PACoCo contains an implementation with a redirect screen. This way, when someone clicks on the active navigation menu item, 
the "OnVisible" code of that screen is run. See my blog post ... for more details. In the companoin app, a button is used to contain 
all "OnVisible" code so that this can be used in that screen too.

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| - | - |
| cmp_OnSelect | This property is related to the OnSelect property of a menu item (the control "lbl_Nav_A_Gall"). It contains a required parameter (cmp_Param_NavID) which contains the ID of the menu item clicked on. |
