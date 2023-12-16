# PACo_SelectList_A

This page is related to version: 2.2

This canvas component is meant to be used for a select list.

![image](https://github.com/formsandflows/PACo/assets/35654198/8ee22ec2-5d31-4fc2-b996-287d5bc77b28)

A select list is used when a selected from one set of values must be made. This component also has a search box which filter the data on values containing the text types in the search box.

## **Input properties**
| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Button | Record | The button to show at the bottom of the panel. | *See the documention on button below.* |
| cmp_SearchReset | Boolean | Used to reset the search box. | true |
| cmp_SelectList | Table | The button to show at the bottom. | *See the documention on select list data below.* |
| cmp_Theme | Record | The theme to use. | *See the documention on theming.* |
| cmp_Visualization | Text | The visualization to use. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | The color of the visualization. | #0078d4 |
| cmp_Width | Number | The the width of the panel. | 400 |

### Button
The button has the following properties:

| Property | Description |
| :--- | :--- |
| Image | A svg definition to be used as an icon. An icon (image) is not required. |
| ImagePadding | The padding of the icon. |
| MinimalWidth | The minimal width of the button. |
| Text | The text to display in the button. |

### Select list data
A gallery is used to show data for the select list. Data consists of records. A record has the following properties:

| Property | Description |
| :--- | :--- |
| Value | The value to show. |

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the property "OnSelect" of the button. |
| cmp_OnSelectListSelect | This property is related to the property "OnSelect" of all select list items. It contains a required parameter (cmp_Param_Value) which contains the value of the select list item clicked on. |
