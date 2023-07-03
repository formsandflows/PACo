Click [here](https://github.com/formsandflows/PACo/blob/main/Releases/Known%20issues.md) for known issues.

## 2023-07-02

Main changes:
* A new canvas component has been added: [PACo_SelectList_A](./../Components/Extra/PACo_SelectList_A.md)
* PACo canvas components with objects containing with a dynamic text width (due to multi-language scenario's) were internally changed and must be used following a specific setup.
* The PACo canvas component [PACo_Button_A](./../Components/Extra/PACo_Button_A.md) has a diffrent setup.
* The help svg icon in the PACo canvas component [PACo_Header_A](./../Components/Core/PACo_Header_A.md) is changed.

| Canvas app | Version | Description |
| :--- | :--- | :--- |
| PACo-Core | [2.2](https://github.com/formsandflows/PACo/raw/main/Releases/PACo-Core%20v2_2.zip) | See [PACo-Core release notes](https://github.com/formsandflows/PACo/blob/main/Releases/PACo-Core_Release%20notes_v2.2.md) |
| PACo-Extra | [2.2](https://github.com/formsandflows/PACo/raw/main/Releases/PACo-Extra%20v2_2.zip) | See [PACo-Extra release notes](https://github.com/formsandflows/PACo/blob/main/Releases/PACo-Extra_Release%20notes_v2.2.md) |
| PACoCo | [2.2](https://github.com/formsandflows/PACo/raw/main/Releases/PACoCo%20v2_2.zip) | See [PACoCo release notes](https://github.com/formsandflows/PACo/blob/main/Releases/PACoCo_Release%20notes_v2.2.md) |
| PACo Examples | [1.2](https://github.com/formsandflows/PACo/raw/main/Releases/PACo%20Examples%20v1_2.zip) | See [PACo Examples release notes](https://github.com/formsandflows/PACo/blob/main/Releases/PACo%20Examples_Release%20notes_v1.2.md) |

## 2023-05-07

The only difference between PACo canvas components v2.0 and v2.1 is related to html controls used to show an elevation visualization.

An update was made to Power Apps resulting in the code in the property "HtmlText" of a html control used to show an elevation visualization to not work anymore. The code in v2.0 contained two hashes (#) before the color value after variable substitution instead of one. This used to work but now not anymore. Having two hashes was the source of the issue and not the Power Apps update.

In all html controls used to show an elevation visualization, the hash is removed from the property "HtmlText". This way, nothing has to be changed in canvas apps using the canvas components.

| Canvas app | Version | Description |
| :--- | :--- | :--- |
| PACo-Core | [2.1](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/PACo-Core%20v2_1.zip) | See [PACo-Core release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/PACo-Core_Release%20notes_v2.0.md) |
| PACo-Extra | [2.1](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/PACo-Extra%20v2_1.zip) | See [PACo-Extra release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/PACo-Extra_Release%20notes_v2.0.md) |
| PACoCo | [2.1](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/PACoCo%20v2_1.zip) | See [PACoCo release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/PACoCo_Release%20notes_v2.0.md) |
| PACo Examples | [1.1](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/PACo%20Examples%20v1_1.zip) | See [PACo Examples release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/PACo%20Examples_Release%20notes_v1.0.md) |

## 2023-05-03

| Canvas app | Version | Description |
| :--- | :--- | :--- |
| PACo-Core | [2.0](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/PACo-Core%20v2_0.zip) | See [PACo-Core release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/PACo-Core_Release%20notes_v2.0.md) |
| PACo-Extra | [2.0](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/PACo-Extra%20v2_0.zip) | See [PACo-Extra release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/PACo-Extra_Release%20notes_v2.0.md) |
| PACoCo | [2.0](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/PACoCo%20v2_0.zip) | See [PACoCo release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/PACoCo_Release%20notes_v2.0.md) |
| PACo Examples | [1.0](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/PACo%20Examples%20v1_0.zip) | See [PACo Examples release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/PACo%20Examples_Release%20notes_v1.0.md) |

## 2023-02-26

| Canvas app | Version | Description |
| :--- | :--- | :--- |
| PACo | [1.2a](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/PACo%20v1_2a.zip) | See [PACo release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/PACo_Release%20notes_v1.2a.md) |
| PACoCo | [1.2a](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/PACoCo%20v1_2a.zip) | See [PACoCo release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/PACoCo_Release%20notes_v1.2a.md) |


## 2022-11-26

| Canvas app | Version | Description |
| :--- | :--- | :--- |
| PACo | [1.1](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/PACo%20v1_1.zip) | See [PACo release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/PACo_Release%20notes_v1.1.md) |
| PACoCo | [1.1](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/PACoCo%20v1_1.zip) | See [PACoCo release notes](https://github.com/formsandflows/PACo/blob/main/Releases/Archive/PACoCo_Release%20notes_v1.1.md) |

## 2022-10-23

| Canvas app | Version | Description |
| :--- | :--- | :--- |
| PACo | [1.0](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/PACo%20v1_0.zip) | Initial release |
| PACoCo | [1.0](https://github.com/formsandflows/PACo/raw/main/Releases/Archive/PACoCo%20v1_0.zip) | Initial release |
