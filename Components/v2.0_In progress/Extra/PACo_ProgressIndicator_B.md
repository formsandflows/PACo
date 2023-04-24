# PACo_ProgressIndicator_B.md

This canvas component is meant to be used for a progress indicator showing process steps of a process.

[[ IMAGE ]]

This version allow for process steps to be skipped. Skipped steps have a disabled full circle.

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_ColorActive | Text | The color used for the current or a previous stage. | #0078d4 |
| cmp_ColorInactive | Text | The color used for an inactive or next stage. | #a19f9d |
| cmp_CurrentStage | Number | The number of the current stage. Numbering starts at 1. | 4 |
| cmp_Items | Table | The process steps. | *See the documention on process steps below.* |
| cmp_TextColor | Text | The color of the text. | #000000 |
| cmp_Theme | Record | The theme to use. | *See the documention on theming.* |
| cmp_Visualization | Text | The visualization to use. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | The color of the visualization. | #0078d4 |

### Process steps

A process step has the following properties:

| Property | Description |
| :--- | :--- |
| ID | The unique number of the process step. Numbering must start at 1 and be sequential. |
| Skip | If the process step must be skipped (inactive) or not. |
| Title | The text to display. |

## **Output properties**

There are no output properties.

## **Behavior properties**

There are no behavior properties.
