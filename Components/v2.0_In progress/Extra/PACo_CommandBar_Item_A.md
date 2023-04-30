# PACo_CommandBar_Item_A

This canvas component is meant to be used for a command bar item.

[[ IMAGE ]]

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Image | Text | A svg definition to be used as an icon. |  |
| cmp_ImagePadding | Number | The padding of the icon. | 10 |
| cmp_Text | Text | The text to show. | "Command 1" |
| cmp_Theme | Record | The theme to use. | *See the documention on theming.* |
| cmp_Title | Text | The internal name of the command bar item. This is needed to support multilingual canvas apps. | "Command1" |

## **Output properties**

| Property | Type | Description |
| :--- | :--- | :--- |
| cmp_Width | Number | The width of the command bar item. |

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the property "OnSelect" of the command bar item (the icon control). |
