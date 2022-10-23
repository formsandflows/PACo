# cmp_Form_A

This canvas component is meant to be used for a form.

![PACo_Form](https://user-images.githubusercontent.com/35654198/197223488-dc2e487e-de05-4a2b-9e3c-cbf3c2c560e5.png)

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Buttons | Table | This property contains the buttons to show on the form. | *See the documention on form buttons below.* |
| cmp_ElevationColor | Text | This property contains the color to use in the elevation of the form. | #0078d4 |
| cmp_FormDefinition | Text | This property contains the form definition. | *See the documention on form definition below.* |
| cmp_Mode | Text | This property determines if a new record must be added or an existing one edited. | New |
| cmp_ResetControls | Boolean | This property is used to reset the form controls | true |
| cmp_Theme | Record | This property contains the theme to use for the form. | *See the documention on theming.* |

### form buttons

A form must shown 2 buttons. A button can be configured with a title and a type (Primary or secondary). The example below is used in the screenshot shown above.

`Table({Title:"Ok", Type:"Primary"}, {Title:"Cancel", Type:"Secondary"})`

### Form definition

A form has two modes:

- Edit
- New

A form can be defined using a fixed setup. [This](./Form%20definition) file contains the form definition used in the companion canvas app [PACoCo](.\\PACoCo.md).

The following properties must be configured per field:

| Property | Description |
| :--- | :--- |
| default | The default value of the field. This is used when the form is used in edit mode. |
| id | The unique ID of the field. |
| name | The display name of the field. |
| required | Of the field is required or not. An asterix is shown before the display name when a field is required. |
| type | The field type. |

The are 4 field types available:

- ComboBoxSingle
- DatePicker
- DropDown
- TextInput

More will be added due time.

The choice values for field of type "ComboBoxSingle" or a "Dropdown" can added to the form definition. The form definition can be dynamically created meaning that for example the choice values can be dynamic and stored outside the canvas app.

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the property "OnSelect" of all form buttons. It contains a required parameter (cmp_Param_Button) which contains the title of the button clicked. It also contains an optional parameter (cmp_Param_Fields) which contains - in case of the "Ok" button - a JSON object containing all field ID's and their values. |
