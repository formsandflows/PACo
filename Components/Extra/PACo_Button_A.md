# PACo_Button_A

This page is related to version: 2.2

This canvas component is meant to be used for a button.

![image](https://user-images.githubusercontent.com/35654198/235982340-10a1d796-453c-45cd-9c4d-4aacc4de5723.png)

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Button | Record | The button to show. | *See the documention on button below.* |
| cmp_Disabled | Boolean | If the button is disabled or not. | false |
| cmp_Theme | Record | The theme to use. | *See the documention on theming.* |

### Button
A button has the following properties:

| Property | Description |
| :--- | :--- |
| Image | A svg definition to be used as an icon. |
| ImagePadding | The padding of the icon. |
| MinimalWidth | The minimal width of the button. |
| Text | The text to display in the button. |
| Type | Possible values: Primary, Secondary. |

## **Output properties**

| Property | Type | Description |
| :--- | :--- | :--- |
| cmp_Width | Number | The calculated width of the button. | 123

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the property "OnSelect" of the button (the icon control). |
