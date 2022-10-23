This canvas component is meant to be used for a dialog.

![image](https://user-images.githubusercontent.com/35654198/197049801-26e700d7-70c2-4742-b8f2-993083c4ab5c.png)

When using variables for the input properties, one dialog component can be used for multiple situations. This is implemented in the companion canvas app [PACoCo](.//PACoCo.md).

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Buttons | Table | This property determines which buttons to show. | *See the documention on buttons below.* |
| cmp_ElevationColor | Text | This property contains the color to use in the elevation of the dialog. | #0078d4 |
| cmp_Message | Text | This property contains the body text of the dialog. | The data will be reloaded. |
| cmp_Percentage | Number | This property contains the percentage of the "border". | 20 |
| cmp_Theme | Record | This property contains the theme to use for the dialog. | *See the documention on theming.* |
| cmp_Title | Text | This property contains the title of the dialog. | Reload |

### Buttons
A dialog can show 1 or 2 buttons depending on its need. A button can be configured with a title and a type (Primary or secondary). The example below is used in the screenshot shown above.

`Table({Title:"Ok", Type:"Primary"}, {Title:"Cancel", Type:"Secondary"})`

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the property "OnSelect" of the buttons. It contains a required parameter (cmp_Param_Button) which contains the title of the button clicked on. |
