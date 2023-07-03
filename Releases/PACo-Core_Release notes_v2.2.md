This page contains the PACo-Core release notes of version 2.2.

| # | Type | Component | Description |
| :---| :--- | :--- | :--- |
| 1 | Change | *Many* | All components have a version in their description. |
| 2 | Update | PACo_Panel_A | The property *cmp_Button* is updated. The property *Title* of the related record is removed. |
| 3 | Change | PACo_CommandBar_B | A more stable setup is used. |
| 4 | Change | PACo_Dialog_A | A more stable setup is used. |
| 5 | Change | PACo_Panel_A | A more stable setup is used. |
| 6 | Update | PACo_Header_A | Another svg is used for help. An i within a circle was used. Now, a question mark wihtin a solid circle is used. |

From version 2, each release has its own numbering for bugs, changes, new features and updates. No continuous numbering is used as was the case prior to version 2.

### #2 - Explanation
A panel contains only one button. The property *OnSelect* will therefore always be related to that button. The property *Title* of the related record was therefore unnecessary. As a consequence, the property *OnSelect* also has no parameter anymore.

### #3, #4, #5 - Explanation
In multi-lingual scenarios, where the width of an object in a component - like the button in the panel component - could change, it was experienced that this change in width did not work consistent. The following changes were therefore made:
* A textinput control was added in the component for every object for which its width could change. The control was hidden.
* The default value of this textinput control was set to the text to display.
* The html control to "calculate" the width of the text to display uses this textinput control.
* The control to display the text uses this textinput control.
* "Raise OnReset when value changes" was selected for the property containing the text to display.
* The property *OnReset* of the component was configured to reset the added textinput control.

## Type description

| Type | Description |
| :--- | :--- |
| Bug | A bug. Something that needed to be fixed. |
| Change | An internal change. No functional change. |
| New feature | A new functionality. |
| Update | An updated functionality. |
