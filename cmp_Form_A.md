This canvas component is meant to be used for a form.

![PACo_Form](https://user-images.githubusercontent.com/35654198/197223488-dc2e487e-de05-4a2b-9e3c-cbf3c2c560e5.png)

## **Input properties**

| Property | Type | Description | Example |
| - | - | - | - |
| cmp_Buttons | Table | This property contains the buttons to show on the form. | *See the documention on form buttons below.* |
| cmp_ElevationColor | Text | This property contains the color to use in the elevation of the form. | #0078d4 |
| cmp_FormDefinition | Text | This property contains the form definition. | *See the documention on form definition below.* |
| cmp_Mode | Text | This property determines if a new record must be added or an existing one edited. | New |
| cmp_ResetControls | Boolean | This property is used to reset the form controls | true |
| cmp_Theme | Record | This property contains the theme to use for the form. | *See the documention on themes.* |

### Form definition


## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| - | - |
| cmp_OnSelect | This property is related to the OnSelect property of all form buttons. It contains two required parameters (cmp_Param_Button and cmp_Param_Fields) which contains the title of the button clicked on and - in case of the "Ok" button - a JSON object containing all field ID's and their values. |
