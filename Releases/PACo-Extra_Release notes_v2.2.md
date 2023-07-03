This page contains the PACo-Extra release notes of version 2.2.

| # | Type | Component | Description |
| :---| :--- | :--- | :--- |
| 1 | Change | *Many* | All components have a version in their description. |
| 2 | Update | PACo_Button_A | Button properties are now configured using a record. This setup is more consistant with other components. |
| 3 | Update | PACo_Button_A | The property *cmp_Title* is removed. |
| 4 | Update | PACo_Button_A | A button changes color when it is disabled, the text color now fits better. This was mostly useful for buttons of type "Secondary". |
| 5 | Update | PACo_CommandBar_Item_A | The property *cmp_Title* is removed. |
| 6 | Change | PACo_Button_A | A more stable setup is used. |
| 7 | Change | PACo_CommandBar_Item_A | A more stable setup is used. |
| 8 | New feature | PACo_SelectList_A | See the component documentation for more details. |

From version 2, each release has its own numbering for bugs, changes, new features and updates. No continuous numbering is used as was the case prior to version 2.

### #2 - Explanation
As a consequence, a new property (*cmp_Button*) was added and several other properties were removed.

### #3, #5 - Explanation
These components contain only one button/item. The property *OnSelect* will therefore always be related to that button/item. The property *cmp_Title* was therefore unnecessary. As a consequence, the property *OnSelect* also has no parameter anymore.

### #6, #7 - Explanation
In multi-lingual scenarios, where the width of an object in a component - like the button in the panel component - could change, it was experienced that this change in width did not work consistent. The following changes were therefore made:
* A textinput control was added in the component for every object for which its width could change. The control was hidden.
* The default value of this textinput control was set to the text to display.
* The html control to "calculate" the width of the text to display uses this textinput control.
* The control to display the text uses this textinput control.
* "Raise OnReset when value changes" was selected for the property containing the text to display.
* The property *OnReset* of the component was configured to reset the added textinput control.

!! To make sure that the corerct width is used, the component properties containing the text to display must use variables. Before the components are shown, the variable must first be given an empty value and then the correct value. This triggers the OnReset of the component making sure the width is calculated properly.

## Type description

| Type | Description |
| :--- | :--- |
| Bug | A bug. Something that needed to be fixed. |
| Change | An internal change. No functional change. |
| New feature | A new functionality. |
| Update | An updated functionality. |
