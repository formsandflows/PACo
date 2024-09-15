# PACo_CommandBar_B

>  [!WARNING]
> This is page contains pre-release information is can be not up-to-date yet. The documention of the latest version is in the archive folder.

This documentation page is related to version: 3.3.0

Related video page: https://www.formsandflows.nl/paco/videos/paco_commandbar_b/

![image](https://github.com/formsandflows/PACo/assets/35654198/7497f77f-6d04-4010-91e6-335a9fd417d1)

A menu indicator (3 dots) is shown when there are commands to show which cannot be shown because the width of the command bar is to small. When the menu indicator is clicked on, the idea is that a command bar menu is shown containing only the commands which are not shown in te command bar. This command bar menu is another PACo canvas component: PACo_CommandBarMenu_A

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_BackgroundColor | Data | Input | Text | The color of the background. | |
| cmp_Commands | Data | Input | Record | The commands. | See the documention about cmp_Commands below. |
| cmp_LastCommand | Data | Output | Number | The last command shown in the command bar. | It contains the related ID. |
| cmp_OnSelect | Event | | None | The event fired when a command is clicked on. | See the documention about cmp_OnSelect below. |
| cmp_SelectedItems | Data | Input | Text | Indicator of the number of selected items (0, 1 or more than 1) in the related details list. | See the documention about cmp_SelectedItems below. |
| cmp_TextStyling | Data | Input | Record | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |

### cmp_Commands
A command has the following properties:

| Property | Description |
| :--- | :--- |
| Disabled | If the command is disabled or not. |
| Hidden | If the command is hidden or not. |
| ID | An unique ID (number) of the command. |
| Image | A svg definition for the image. |
| ImagePadding | The padding of the image. |
| SelectedItems | When to show the command. See the documention about cmp_SelectedItems below. |
| Text | The text. |
| TextPaddingLeft | The padding left of the text. |
| TextPaddingRight | The padding right of the text. |

This component allows for up to 8 commands.

### cmp_OnSelect
This custom property contains a required parameter called "cmp_Param_CommandID" which contains the ID of the command clicked on. When the menu indicator is clicked on, a 0 (zero) is returned.

### cmp_SelectedItems
A command can be shown for the situations when 0, 1 or more than 1 items are selected in the related details list canvas component. There are 3 details list canvas components (PACo_DetailsList_A, PACo_DetailsList_B, PACo_DetailsList_C) part of PACo.

To make this possible, a fixed setup must be followed for the property "SelectedItems" of a command and for the custom property "cmp_Selecteditems" of the canvas component.

#### Property "SelectedItems" of a command bar item
This property is used to determine when the command must be shown.

- #0# > The command is shown when no items are selected in the details list.
- #1# > The command is shown when 1 item is selected in the details list.
- #2# > The command is shown when more than 1 item is selected in the details list.

Above are example of single situations. The property "SelectedItems" of a command can also be used for multiple situations. Example: A command which has "#0#1#2#" set for its property "SelectedItems" is shown for the situations when 0, 1 or more than 1 item is selected in the details list.

#### Custom property "cmp_SelectedItems" of the component
This property determines if 0, 1 or more than 1 items are selected in the details list.

- #0# > Commands with "#0#" in their property "SelectedItems" are shown.
- #1# > Commands with "#1#" in their property "SelectedItems" are shown.
- #2# > Commands with "#2#" in their property "SelectedItems" are shown.

### cmp_TextStyling
This custom property has the following properties:

| Property | Description |
| :--- | :--- |
| Color | The color. |
| Font | The font. |
| FontSize | The font size. |
