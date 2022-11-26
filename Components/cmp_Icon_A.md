# cmp_Tile_A

This canvas component is meant to be used for an icon.

![image](https://user-images.githubusercontent.com/35654198/204077593-0f53ebd9-d6de-4937-b1a2-774a08c8603c.png)

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_Disabled | Boolean | This property determines if the icon is disabled. | false |
| cmp_Icon | Record | This property contains the icon to show. | *See the documention on the icon below.* |
| cmp_Theme | Record | This property contains the theme to use for the panel. | *See the documention on theming.* |
| cmp_Visualization | Text | This property contains the visualization. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | This property contains the color to use in the visualization. | #0078d4 |

### The icon
To be able to change the icon, a component of type "Record" has to be used. The record has the following structure:

| Property | Description |
| :--- | :--- |
| Icon | The icon to show. |

Example:
{icon: Icon.Add}

## **Output properties**

There are no output properties.

## **Behavior properties**

| Property | Description |
| :--- | :--- |
| cmp_OnSelect | This property is related to the propertu "OnSelect" of the icon. |
