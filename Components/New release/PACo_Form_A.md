# PACo_Form_A

This canvas component is:

- meant to be used for a form.
- still in development. Not many field types are supported and I experience also some quirks. That is why, for now, creating your own forms - with the visualization canvas component if needed - is the prefererd way to implement forms.

![PACo_Form](https://user-images.githubusercontent.com/35654198/197223488-dc2e487e-de05-4a2b-9e3c-cbf3c2c560e5.png)

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Buttons | Table | This property contains the buttons to show on the form. | *See the documention on form buttons below.* |
| cmp_FormDefinition | Text | This property contains the form definition. | *See the documention on form definition below.* |
| cmp_Mode | Text | This property determines if a new record must be added or an existing one edited. | New |
| cmp_ResetControls | Boolean | This property is used to reset the form controls. | true |
| cmp_Theme | Record | This property contains the theme to use for the form. | *See the documention on theming.* |
| cmp_Visualization | Text | This property contains the visualization. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | This property contains the color to use in the visualization. | #0078d4 |

### Form buttons

A form has 2 buttons. A button has the following properties:

| Property | Description |
| :--- | :--- |
| Text | The text to display in the button. |
| Title | The internal name of the button. This is needed to support multilingual canvas apps. |
| Type | Possible values: Primary or secondary. |
| Width | The width of the button. |

The example below is used in the screenshot shown above.

Table({Text:"Ok", Title:"Ok", Type:"Primary", Width:160}, {Text:"Cancel", Title:"Cancel", Type:"Secondary", Width:160})

### Form definition

A form has two modes:

- Edit
- New

A form can be defined using a fixed setup. [This](./Form%20definition) file contains the form definition used in the companion canvas app [PACoCo](./../PACoCo.md).

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
  - No theming support.
- DropDown
- TextInput

More field types will be added in the future.

The choice values for field of type "ComboBoxSingle" or a "Dropdown" can added to the form definition. The form definition can be dynamically created meaning that for example the choice values can be dynamic and stored outside the canvas app.

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the property "OnSelect" of all form buttons. It contains a required parameter (cmp_Param_Button) which contains the title of the button clicked. It also contains an optional parameter (cmp_Param_Fields) which contains - in case of the "Ok" button - a JSON object containing all field ID's and their values. |
