# PACoCo

PACoCo is the companion canvas app for PACo. Where PACo only contains canvas components, PACoCo is a canvas app using these canvas components. PACoCo can be regarded as a reference canvas app meaning people can use it to investigate in detail how the components can be used.

![PACo_Template](https://user-images.githubusercontent.com/35654198/197381788-22ae1153-3599-4836-a67c-3d9c28566f79.png)

The backlog of PACo is [here](https://www.formsandflows.nl/pacoco-backlog/).

## Data
PACoCo contains a collection of 50000 items which were imported using “Import from Excel”. Each item represents a sales record. This data, and more 100% copyright free test data, is offered [here](https://excelbianalytics.com/wp/downloads-18-sample-csv-files-data-sets-for-testing-sales/).

PACoCo uses only a portion of this data though and well data that complies to:
- Region = Europe
- Country = The Netherlands

## Functionalities

This section gives a high-level overview of the functionalities of PACoCo:

- When a user starts PACoCo, the code in the button "btn_Start" is executed. It contains code that needs to be run only once per app start.
- Then, the user is navigated to the screen "Home Screen".
- The image shown above is how the home screen looks like.
- When a user clicks on a navigation item, (s)he is navigated to the related screen. Only the home screen has implemented many components though.
- The items in the command bar depend on the amount of selected items (0, 1 or more than 1).
  - New > Add a new item
  - Edit > Edit the selected item
  - Delete > Delete the selected item(s). A dialog box is shown first.
  - Reload > Data is reloaded as if the app had just started. A dialog box is shown first.
- The checkbox in the header can be used to select/unselect all shown items. Items not shown because of a filter are not selected/unselected.
- The first four header column can be clicked on to set its sorting.
  - A user can click the header again to change to sorting (Ascending, Descending, None).
  - You can configure which column can be used for sorting.
  - Only one column can be used for sorting.
- The width of a header column is fixed but can be configured.
- When the total width of the columns is more wide than the available space, a horizontal scrollbar is shown.
- The items shown in the details list can be filtered with the seach box. Only the first column is used for filtering.
  - Multiple columns can be used for filtering if needed.
- When an item is clicked on, a panel is shown containing all properties to show.
  - The panel has an edit and delete command which is related to the same commands in the command bar.
- The header contains a help icon which has no active code behind it.
- The header contains a settings icon to show a settings menu.
- The settings menu has one item: Theme
  - A settings menu can have multiple items.
- The setting "Theme" navaigates a user to the theme screen from where a theme (Default, Dark, High-contract or Fluent UI) can be selected.
- The header of the theme screen contains a back icon to navigate back to the home screen.

## Responsiveness

PACoCo is a responsive app with the following setup:

- The minimum width of a screen is 1024. When the screen width is less, a horizontal scrollbar is shown.
- There is no maximum width for a screen. The app has a maximum width of 1800 though. This means that when a screen width is larger than 1800, the app width is 1800 and shown horizontal centered.
- The minum height of a screen is 640. When the screen height is less, a vertical scrollbar (and therefor also a horizontal scrollbar) is shown .

## Screens
There are three special screens in PACoCo which need some extra explanation:
- Color Screen
- Redirect Screen
- Start Screen

The other screens are accessible when running the canvas app.

### Color screen
This screen is only visible in edit mode and it contains a block per palette slot. See [Theming](./theming.md) for more information on palette slots. A block contains the name of the palette slot and its related color code. The color of the text is set to its color property. The actual values depend on the active theme. For example, theme "Default" will show:

![image](https://user-images.githubusercontent.com/35654198/197279296-d19ede43-3529-4df5-a7a8-476d3aa59e30.png)

### Redirect screen
The [navigation](cmp_Nav_A.md) has the following setup:

1. Each navigation item (menu item) is related to a dedicated screen.
2. When a navigation item is clicked on, the current screen is configured in the global variable "glb_RedirectScreen".
3. The user is then navigated to the screen “Redirect Screen”.
4. The property "Onvisible" of the redirect screen has one line of code which selects the button "btn_Redirect".
5. The property "OnSelect" of the button "btn_Redirect" has code to redirect the logged in user to the screen set in the global variable "glb_RedirectScreen".

With this setup, the property "OnVisible" of the clicked on navigation item is run again. You can implement you own setup on how to deal with the navigation of course.

The following blog post gives more input: [Run your screen’s "OnVisible" code again with a redirect screen](https://www.formsandflows.nl/2022/08/27/run-your-screens-onvisible-code-again-with-a-redirect-screen/)

To be able to change the code in the property "OnSelect" of the button "btn_Redirect", one line of code is added to the property "OnStart" of the "App" object:

`Set(glb_Redirect, true)`

When setting this global variable to false and then running App.OnStart, the user is not navigated back to the screen in the global variable "glb_RedirectScreen" and the code in button "btn_Start" can be changed to your liking.

### Start screen
The start screen is the screen started when the app is started. The property "Onvisible" of the start screen has one line of code which selects the button "btn_Start". The property "OnSelect" of the button "btn_Start" has code which needs to be run only once. At the end of the code, the user is navigated to the home screen.

With this setup, the user starting the app sees a spinner as soon as possible.

To be able to change the code in the property "OnSelect" of the button "btn_Start", one line of code is added to the property "OnStart" of the "App" object:

`Set(glb_Redirect, true)`

When setting this global variable to false and then running App.OnStart, the user is not navigated to the home screen and the code in button "btn_Start" can be changed to your liking.
