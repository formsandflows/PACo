# PACo_ProgressIndicator_A

This page is related to version: 2.2

This canvas component is meant to be used for a progress indicator showing process steps of a process.

![image](https://user-images.githubusercontent.com/35654198/235982695-d096187d-845d-450e-a67e-ebf863688f5b.png)

This version does not allow for process steps to be skipped.

## **Input properties**

| Property | Type | Description | Example |
| :--- | :--- | :--- | :--- |
| cmp_ColorActive | Text | The color used for the current or a previous stage. | #0078d4 |
| cmp_ColorInactive | Text | The color used for a next stage. | #a19f9d |
| cmp_CurrentStage | Number | The number of the current stage. Numbering starts at 1. | 4 |
| cmp_Items | Table | The process steps. | *See the documention on process steps below.* |
| cmp_TemplateSize | Number | The related property of the gallary used. | 120 |
| cmp_TextColor | Text | The color of the text. | #000000 |
| cmp_Theme | Record | The theme to use. | *See the documention on theming.* |
| cmp_Visualization | Text | The visualization to use. | *See the documention on the component cmp_Visualization_A.* |
| cmp_VisualizationColor | Text | The color of the visualization. | #0078d4 |

### Process steps

A process step has the following properties:

| Property | Description |
| :--- | :--- |
| ID | The unique number of the process step. Numbering must start at 1 and be sequential. |
| Title | The text to display. |

## **Output properties**

There are no output properties.

## **Behavior properties**

There are no behavior properties.
