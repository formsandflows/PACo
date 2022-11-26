# cmp_SearchBox_A

This canvas component is meant to be used for a search box.

![PACo_SearchBox](https://user-images.githubusercontent.com/35654198/197222952-adf0cb05-25cc-4084-8d4a-9496a88ee0d0.png)

The search box can be used to filter the items shown in the details list component.

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_HintText | Text | This property is used to set the hint text to show. | Search |
| cmp_Reset | Boolean | This property is used to reset the search box | true |
| cmp_Theme | Record | This property contains the theme to use for the command bar. | *See the documention on theming.* |
| cmp_Visualization | Text | This property contains the visualization. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | This property contains the color to use in the visualization. | #0078d4 |

## **Output properties**

| Property | Type | Description |
| :--- | :--- | :--- |
| cmp_Text | Text | This property contains the text typed into the search box. |

## **Behavior properties**

There are no behavior properties.
