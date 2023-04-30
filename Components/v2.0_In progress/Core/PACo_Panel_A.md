# PACo_Panel_A

This canvas component is meant to be used for a panel.

[[ IMAGE ]]

A panel is shown when an item in the details list component is clicked on. This must be configured in the details list component! With a panel, normally all data is shown meaning more item properties than the ones shown in the details list component. A vertical scrollbar appears when there is more data to show than fits on the screen.

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Button | Record | The button to show at the bottom of the panel. | *See the documention on panel button below.* |
| cmp_Commands | Record | The panel command bar items to show in the top of the panel. | *See the documention on panel command bar items below.* |
| cmp_ImagePadding | Number | The padding of the icons. | 10 |
| cmp_Records | Table | The data to show in the panel. | *See the documention on panel data below.* |
| cmp_Theme | Record | The theme to use. | *See the documention on theming.* |
| cmp_Visualization | Text | The visualization to use. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | The color of the visualization. | #0078d4 |
| cmp_Width | Number | The the width of the panel. | 400 |

### Panel button

The panel button has the following properties:

| Property | Description |
| :--- | :--- |
| Image | A svg definition to be used as an icon. An icon (image) is not required. |
| MinimalWidth | The minimal width of the button. |
| Text | The text to display in the button. |
| Title | The internal name of the button. This is needed to support multilingual canvas apps. |

### Panel command bar items
A panel command bar item has the following properties:

| Property | Description |
| :--- | :--- |
| ID | An unique ID (number) of the command bar item. |
| Image | A svg definition to be used as an icon. |
| Text | The text to display in the related label control. |
| Title | The internal name of the panel command bar item. This is needed to support multilingual canvas apps. |

A maximum of 2 commands are supported (read: configured/tested)!

When the property "Text" has no value, the related panel command bar item is not shown.

### Panel data
A gallery is used to show data in the panel. Data consists of records. A record has the following properties:

| Property | Description |
| :--- | :--- |
| Label | The label text. |
| LabelHeight | The height of the label. |
| Text | The gallery item text. |
| TextHeight | The height of the gallery item. |

The LabelHeight and TextHeight properties are not required. A value of 40 is used in case the properties are not defined.

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnCommandSelect | This property is related to the property "OnSelect" of all panel command bar items. It contains a required parameter (cmp_Param_Command) which contains the title of the command item clicked on. |
| cmp_OnSelect | This property is related to the property "OnSelect" of the panel button. |
