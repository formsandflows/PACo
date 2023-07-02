# PACo_Button_A

This canvas component is meant to be used for a button.

![image](https://user-images.githubusercontent.com/35654198/235982340-10a1d796-453c-45cd-9c4d-4aacc4de5723.png)

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Disabled | Boolean | If the button is disabled or not. | false |
| cmp_Image | Text | A svg definition to be used as an icon. |  |
| cmp_ImagePadding | Number | The padding of the icon. | 10 |
| cmp_MinimalWidth | Number | The minimal width of the button. | 100 |
| cmp_Text | Text | The text to show. | "Button X" |
| cmp_Theme | Record | The theme to use. | *See the documention on theming.* |
| cmp_Title | Text | The internal name of the button. This is needed to support multilingual canvas apps. | "ButtonX" |
| cmp_Type | Text | The type of button (Primary, Secondary). | "Primary" |

## **Output properties**

| Property | Type | Description |
| :--- | :--- | :--- |
| cmp_Width | Number | The calculated width of the button. | 123

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the property "OnSelect" of the button (the icon control). |
