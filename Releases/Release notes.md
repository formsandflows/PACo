Click [here](https://www.formsandflows.nl/redirects/paco-github-known-issues) for known issues.

Click [here](https://www.formsandflows.nl/redirects/paco-github-backlog) for change requests (backlog).

Click [here](https://github.com/formsandflows/PACo/blob/main/Releases/Release%20notes_Canvas%20components_Versions.md) for an overview of canvas component versions per release (from release 3.3.0).

## Release 3.4.0 (2024-10-25)

* [Managed solution](https://github.com/formsandflows/PACo/raw/main/Releases/PACo_3.4.0_Managed.zip) version: 2023.0.0.46
* [Unmanaged solution](https://github.com/formsandflows/PACo/raw/main/Releases/PACo_3.4.0_Unmanaged.zip) version: 2023.0.0.45

The following updates are part of this release:
* 1 new canvas component:
  * **PACo_Breadcrumb_A**
* The canvas component "PACo_InformationBlock_A" now has an option (using adjustable images) to open/close the information block. When an information block is closed, the title is still visible.
* Because of this, the canvas component "PACo_InformationBlock_A" has 4 extra custom properties:
  * cmp_Collapsed
  * cmp_ChevronStyling
  * cmp_OnSelectChevron
  * cmp_TitleHeight
* The canvas app "PACo Examples" is extended with a new screen for this new canvas component.
* The controls in the canvas app "PACo Examples" are changed (where needed) to be standardized.

## Release 3.3.0 (2024-09-28)

* [Managed solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.3/PACo_3.3.0_Managed.zip) version: 2023.0.0.44
* [Unmanaged solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.3/PACo_3.3.0_Unmanaged.zip) version: 2023.0.0.43

The following updates are part of this release:
* 1 new canvas component:
  *  **PACo_PeoplePicker_A**
* The canvas app "PACo Examples" is extended with a new screen for this new canvas component. The screen for "PACo_InformationBlock_A" has been extended with a second load button to see the difference between using auto height or not.
* The canvas components "PACo_HeaderSettingsMenu_A" and "PACo_Nav_B" have a new property in the custom property "cmp_Nav": Hidden
* The way to hide an item in the canvas components mentioned above is applied to the canvas components "PACo_CommandBar_B" and "PACo_Tabs_A". As a result:
  * the custom property "cmp_Authorization" is removed on these canvas components.
  * the canvas components "PACo_CommandBarMenu_A" and "PACo_TabsMenu_A" also have a property "Hidden".
*  A GitHub page containing the canvas component versions per release (from this release).
*  All canvas components containing a container have the border radius set to 0 instead of 4. That's why in this release several canvas components have a new version without any functional change.
*  The canvas component "PACo_InformationBlock_A" has an extra custom property:
  * cmp_AutoHeight
* The canvas component "PACo_SelectList_A" has a new default button. It shows "Cancel" and is of type "Secondary" (instead of showing "Ok" and being of type "Primary").

## Release 3.2.1 (2024-07-29)

* [Managed solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.2/PACo_3.2.1_Managed.zip)
* [Unmanaged solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.2/PACo_3.2.1_Unmanaged.zip)

The canvas component "PACo_InformationBlock_A" now only has a divider between the title and the rest of the information (as intended).

## Release 3.2.0 (2024-07-29)

* [Managed solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.2/PACo_3.2.0_Managed.zip)
* [Unmanaged solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.2/PACo_3.2.0_Unmanaged.zip)

### Feature requests:
* CR-2024-8
* CR-2024-10
* CR-2024-11
* CR-2024-12
* CR-2024-13
* CR-2024-14
* CR-2024-15
* CR-2024-16
* CR-2024-18

### Issues:
* I-2024-8
* I-2024-9
* I-2024-10

The following updates are part of this release:
* 3 new canvas components:
  * **PACo_InformationBlock_A**
  * **PACo_ProgressIndicator_E**
  * **PACo_ProgressIndicator_F**
* Almost all canvas components now have the custom property "cmp_BackgroundColor".
* All canvas components having a divider between items/records, now have the custom property "cmp_DividerColor".
* All shimmers now have the custom property "cmp_ShimmerColor".
* For many controls in many canvas components, the property "Fill" is set to transparent instead of the palette slot "white".
* The alignment of the text controls of commands (PACo_CommandBar_B, PACo_CommandBar_Item_A & PACo_Panel_A) is set to left.
* The details list canvas components have the option to configure the:
  * the checkbox color.
  * the header background color.
  * the header divider color.
* The details list canvas components have a new sorting icon. The color of the icon can ce configured.
* The progress indicator canvas components have a new custom property:
  * cmp_OnSelect
* The progress indicator canvas components have a new setting in the custom property "cmp_Items":
  * Clickable
* All custom properties of type "Event" and "Action" now have a return data type of: None
  * As a consequece, the custom properties are not shown anymore in the panel. They can still be selected in the property selector in the top left.
* PACo_Info_A
  * A new custom property: cmp_TextBorderColor
* PACo_Panel_A
  * A new custom property: cmp_OnSelectNotPanel
  * A new custom property: cmp_OnSelectNotPanelClickable
  * A new custom property: cmp_BackgroundColorCommandBar
* PACo_SearchBox_A
  *  A new custom property: cmp_IconColor
* PACo_SelectList_A
  * A new custom property: cmp_BackgroundColorSearchBox
  * A new custom property: cmp_BackgroundColorList
  * A new custom property: cmp_IconColor
* PACo_Tabs_A
  * A new custom property: cmp_Authorization
  * A new custom property: cmp_SelectedColor
* PACo_TabsMenu_A
  * A new custom property: cmp_Authorization
  * A new custom property: cmp_SelectedColor
* The canvas component documentation pages are updated so that custom properties of type "Table", now have a section for all records in the table, with the options for that record l records instead of one table with all possible options for all records. Example: canvas component "PACo_Panel_A" custom property "cmp_TextStyling".

## Release 3.1.0 (2024-03-18)

* [Managed solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.1/PACo_3.1.0_Managed.zip)
* [Unmanaged solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.1/PACo_3.1.0_Unmanaged.zip)

### Feature requests:
* CR-2023-1
* CR-2024-1
* CR-2024-2
* CR-2024-3
* CR-2024-4
* CR-2024-5
* CR-2024-6
* CR-2024-7
* CR-2024-9

### Issues:
* I-2024-4
* I-2024-5
* I-2024-6
* I-2024-7

The following updates are part of this release:

* PACo_Button_A
  * An updated custom property "cmp_TextStyling".
* PACo_CommandBar_B
  * A new custom property called "cmp_Authorization".
* PACo_CommandBarMenu_A
  * A new custom property called "cmp_Authorization".
* PACo_DetailsList_A
  * A new custom property called "cmp_CheckboxStyling".
  * A new custom property called "cmp_HeaderStyling".
  * A new custom property called "cmp_ShowHoverFill".
  * A new custom property called "cmp_SortingIconStyling".
  * A different way of working for custom property "cmp_ShowCheckbox".
  * An updated custom property "cmp_TextStyling".
  * The custom property "cmp_ShowCheckboxHeader" is removed.
* PACo_DetailsList_B
  * See canvas component "PACo_DetailsList_A".
* PACo_Dialog_A
  * An updated custom property "cmp_TextStyling".
* PACo_Panel_A
  * An updated custom property "cmp_TextStyling".
    * The property "Color" must now also be set for the item related to the button in the custom property "cmp_TextStyling".
* PACo_ProgressIndicator_A
  * A new custom property called "cmp_Offset".
  * A new custom property called "cmp_ShowText".
  * An updated custom property "cmp_TextStyling".
* PACo_ProgressIndicator_B
  * The same as canvas component "PACo_ProgressIndicator_A".
* PACo_SelectList_A
  * An updated custom property "cmp_TextStyling".
    * The property "Color" must now also be set for the item related to the button in the custom property "cmp_TextStyling".

## Release 3.0.6 (2024-01-28)

* [Managed solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.0/PACo_3.0.6_Managed.zip)
* [Unmanaged solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.0/PACo_3.0.6_Unmanaged.zip)

### Issue:
* I-2024-3

## Release 3.0.5 (2024-01-06)

* [Managed solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.0/PACo_3.0.5_Managed.zip)
* [Unmanaged solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.0/PACo_3.0.5_Unmanaged.zip)

### Issues:
* I-2024-1
* I-2024-2

## Release 3.0.4 (2023-12-29)

* [Managed solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.0/PACo_3.0.4_Managed.zip)
* [Unmanaged solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.0/PACo_3.0.4_Unmanaged.zip)

### Issue:
* I-2023-6

## Release 3.0.3 (2023-12-28)

* [Managed solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.0/PACo_3.0.3_Managed.zip)
* [Unmanaged solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.0/PACo_3.0.3_Unmanaged.zip)

### Issue:
* I-2023-5

## Release 3.0.2 (2023-12-28)

* [Managed solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.0/PACo_3.0.2_Managed.zip)
* [Unmanaged solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.0/PACo_3.0.2_Unmanaged.zip)

### Feature requests:
* CR-2023-3
* CR-2023-4
* CR-2023-5 

### Issues:
* I-2023-3
* I-2023-4

## Release 3.0.1 (2023-12-24)

* [Managed solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.0/PACo_3.0.1_Managed.zip)
* [Unmanaged solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.0/PACo_3.0.1_Unmanaged.zip)

### Feature request:
* CR-2023-2

### Issues:
* I-2023-1
* I-2023-2

## Release 3.0.0 (2023-12-19)

* [Managed solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.0/PACo_3.0.0.Managed.zip)
* [Unmanaged solution](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v3.0/PACo_3.0.0_Unmanaged.zip) 

### Main changes
* Improved release management:
  * Regular (quarterly) releases.
  * Hotfix releases.
  * Versoning.
* Extended documentation.
* Paid support.
* Almost all canvas components now have a custom property "cmp_TextStyling" to change how the text is displayed.
* Canvas component PACo_Header_A:
  * The option for a (clickable) logo is added.
  * The option for a language selector is added.
* Four new canvas components (26 in total):
  * PACo_HeaderLanguagesMenu_A
  * PACo_Log_A
  * PACo_Tabs_A
  * PACo_TabsMenu_A
* PACo Examples:
  * Examples for the new canvas components.
* PACoCo:
  * Responsiveness additions/improvements.
  * A simplified multi-language implementation.
  * The new canvas components "PACo_HeaderLanguagesMenu_A", "PACo_Tabs_A" and "PACo_TabsMenu_A" are included.
  * Using App.Formulas and named formulas instead of App.OnStart.
* Logic (code) simplifications.
* PACo is added with a Power Platform solution.
  * A managed solution and an unmanaged solution are provided.
* The canvas components are now offered using a component library.

## Release 2.2 (2023-07-02)
### Main changes
* A new canvas component has been added: PACo_SelectList_A
* PACo canvas components with objects containing with a dynamic text width (due to multi-language scenario's) were internally changed and must be used following a specific setup.
* The PACo canvas component PACo_Button_A has a diffrent setup.
* The help svg icon in the PACo canvas component PACo_Header_A is changed.

| Canvas app | Version | Description |
| :--- | :--- | :--- |
| PACo-Core | [2.2](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v2.2/PACo-Core%20v2_2.zip) | See [PACo-Core release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/v2.2/PACo-Core_Release%20notes_v2.2.md) |
| PACo-Extra | [2.2](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v2.2/PACo-Extra%20v2_2.zip) | See [PACo-Extra release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/v2.2/PACo-Extra_Release%20notes_v2.2.md) |
| PACoCo | [2.2](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v2.2/PACoCo%20v2_2.zip) | See [PACoCo release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/v2.2/PACoCo_Release%20notes_v2.2.md) |
| PACo Examples | [1.2](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v2.2/PACo%20Examples%20v1_2.zip) | See [PACo Examples release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/v2.2/PACo%20Examples_Release%20notes_v1.2.md) |

## Release 2.1 (2023-05-07)
The only difference between PACo canvas components v2.0 and v2.1 is related to html controls used to show an elevation visualization.

An update was made to Power Apps resulting in the code in the property "HtmlText" of a html control used to show an elevation visualization to not work anymore. The code in v2.0 contained two hashes (#) before the color value after variable substitution instead of one. This used to work but now not anymore. Having two hashes was the source of the issue and not the Power Apps update.

In all html controls used to show an elevation visualization, the hash is removed from the property "HtmlText". This way, nothing has to be changed in canvas apps using the canvas components.

| Canvas app | Version | Description |
| :--- | :--- | :--- |
| PACo-Core | [2.1](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v2.1/PACo-Core%20v2_1.zip) | See [PACo-Core release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/v2.0/PACo-Core_Release%20notes_v2.0.md) |
| PACo-Extra | [2.1](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v2.1/PACo-Extra%20v2_1.zip) | See [PACo-Extra release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/v2.0/PACo-Extra_Release%20notes_v2.0.md) |
| PACoCo | [2.1](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v2.1/PACoCo%20v2_1.zip) | See [PACoCo release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/v2.0/PACoCo_Release%20notes_v2.0.md) |
| PACo Examples | [1.1](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v2.1/PACo%20Examples%20v1_1.zip) | See [PACo Examples release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/v2.0/PACo%20Examples_Release%20notes_v1.0.md) |

## Release 2.0 (2023-05-03)

| Canvas app | Version | Description |
| :--- | :--- | :--- |
| PACo-Core | [2.0](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v2.0/PACo-Core%20v2_0.zip) | See [PACo-Core release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/v2.0/PACo-Core_Release%20notes_v2.0.md) |
| PACo-Extra | [2.0](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v2.0/PACo-Extra%20v2_0.zip) | See [PACo-Extra release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/v2.0/PACo-Extra_Release%20notes_v2.0.md) |
| PACoCo | [2.0](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v2.0/PACoCo%20v2_0.zip) | See [PACoCo release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/v2.0/PACoCo_Release%20notes_v2.0.md) |
| PACo Examples | [1.0](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v2.0/PACo%20Examples%20v1_0.zip) | See [PACo Examples release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/v2.0/PACo%20Examples_Release%20notes_v1.0.md) |

## Release 1.2a (2023-02-26)

| Canvas app | Version | Description |
| :--- | :--- | :--- |
| PACo | [1.2a](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v1.2a/PACo%20v1_2a.zip) | See [PACo release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/v1.2a/PACo_Release%20notes_v1.2a.md) |
| PACoCo | [1.2a](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v1.2a/PACoCo%20v1_2a.zip) | See [PACoCo release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/v1.2a/PACoCo_Release%20notes_v1.2a.md) |


## Release 1.1 (2022-11-26)

| Canvas app | Version | Description |
| :--- | :--- | :--- |
| PACo | [1.1](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v1.1/PACo%20v1_1.zip) | See [PACo release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/v1.1/PACo_Release%20notes_v1.1.md) |
| PACoCo | [1.1](https://github.com/formsandflows/PACo/raw/main/Releases/v1.1/Archive/PACoCo%20v1_1.zip) | See [PACoCo release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/v1.1/PACoCo_Release%20notes_v1.1.md) |

## Release 1.0 (2022-10-23)
Initial release
| Canvas app | Version | Description |
| :--- | :--- | :--- |
| PACo | [1.0](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v1.0/PACo%20v1_0.zip) | Initial release |
| PACoCo | [1.0](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/v1.0/PACoCo%20v1_0.zip) | Initial release |
