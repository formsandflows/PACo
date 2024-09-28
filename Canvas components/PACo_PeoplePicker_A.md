# PACo_PeoplePicker_A

>  [!WARNING]
> This is page contains pre-release information is can be not up-to-date yet. The documention of the latest version is in the archive folder.

This documentation page is related to version: 3.3.0

![image](https://github.com/user-attachments/assets/af7a56d3-fe80-4161-8e8d-81c349403b06)

This canvas component has its "OnReset" property configured. When a canvas component instance is reset, the text input control is reset.

## Custom properties

| Display name | Property type | Property definition | Data type | Description | Memo
| :--- | :--- | :--- | :--- | :--- | :--- |
| cmp_BackgroundColor | Data | Input | Text | The color of the background. | |
| cmp_BackgroundColorSearchBox | Data | Input | Text | The color of the search box background. | |
| cmp_BackgroundColorUsers | Data | Input | Text | The color of the users background. | |
| cmp_Button | Data | Input | Record | The button at the bottom of the panel. | See the documention about cmp_Button below. |
| cmp_DividerColor | Data | Input | Text | The color of the divider. | |
| cmp_IconColor | Data | Input | Text | The color of the icons. | |
| cmp_Office365Users | Data | Input | Table | The users to show. | See the documention about cmp_Office365Users below. |
| cmp_OnSelect | Event | | None | The event fired when the button is clicked on. | |
| cmp_OnOffice365User | Event | | None | The event fired when an Office 365 user is clicked on. | See the documention about cmp_OnOffice365User below. |
| cmp_Properties | Data | Input | Record | The properties configuration.| See the documention about cmp_Properties below. |
| cmp_Text | Data | Output | Text | Contains the text typed into the search box. | |
| cmp_TextStyling | Data | Input | Table | Text properties. | See the documention about cmp_TextStyling below. |
| cmp_Theme | Data | Input | Record | The theme. | See the documention on theming. |
| cmp_Visualization | Data | Input | Text | The visualization. | See the documention of PACo canvas component PACo_Visualization_A. |
| cmp_VisualizationColor | Data | Input | Text | The color of the visualization. | |
| cmp_Width | Data | Input | Number | The width of the panel. | |

### cmp_Button
The button has the following properties:

| Property | Description |
| :--- | :--- |
| Border | If a border must be shown. This only applies to a button of type "Secondary". |
| BorderRadius | The radius of the border of the button. |
| Height | The height.|
| Image | A svg definition for an image. An image is not required. |
| ImagePadding | The padding of the image. |
| MinimalWidth | The minimal width. |
| Text | The text. |
| Type | The button type. Possible values are "Primary" and "Secondary". |

### cmp_Office365Users
A user has the following properties:

| Property | Description |
| :--- | :--- |
| Department | The depertment of the user. |
| DisplayName | The display name of the user. |
| Mail | The email address of the user. |

### cmp_OnSelectListItem
This custom property contains a required parameter called "cmp_Param_Value" which is of type "Record" and contains the user properties of the user clicked on.

### cmp_Properties
With this custom property configures the properties to show and how to show them (Property1 only).

Property1: Display name or display name and email address between parentheses
Property2: Email address
Property3: Department

| Property | Description |
| :--- | :--- |
| Property1 | The text to show for the label. |
| Property1Type | The property1 type. Possible values: "DisplayName" and "DisplayNameMail". |
| Property2 | The text to show for the label. |
| Property3 | The text to show for the label. |
| ShowProperty1 | If property1 must be shonw. |
| ShowProperty2 | If property2 must be shonw. |
| ShowProperty3 | If property3 must be shonw. |

### cmp_TextStyling
This custom property is of data type "**Table**" and has the following records:

#### Button

| Property | Description |
| :--- | :--- |
| Color | The color. |
| ID | The value: Button |
| Font | The font. |
| FontSize | The font size. |

#### PeoplePicker

| Property | Description |
| :--- | :--- |
| Align | The horizontal alignment. |
| Color | The color. |
| ID | The value: PeoplePickerItem |
| Font | The font. |
| FontSize | The font size. |
| FontStyle | The font style. Possible values are: "" and "Italics" |
| FontWeight | The font weight. |
| Padding | The padding. |
| VerticalAlign | The vertical alignment. |

#### PeoplePickerLabel

| Property | Description |
| :--- | :--- |
| Align | The horizontal alignment. |
| Color | The color. |
| ID | The value: PeoplePickerItem |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| Padding | The padding. |
| VerticalAlign | The vertical alignment. |

#### Search

| Property | Description |
| :--- | :--- |
| Align | The horizontal alignment. |
| Color | The color. |
| ID | The value: Search |
| Font | The font. |
| FontSize | The font size. |
| FontWeight | The font weight. |
| Padding | The padding. |
| TextBlockHeight | The height of the text block. |
