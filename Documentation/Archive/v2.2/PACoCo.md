# PACoCo

PACoCo is the companion canvas app to demonstrate how several PACo canvas components can be used together. PACoCo can be regarded as a reference canvas app meaning people can use it to investigate in more detail how the components can be used.

![image](https://user-images.githubusercontent.com/35654198/235985153-9a98897d-715f-46b8-8f3a-d28be2fdfaa4.png)

## Data
PACoCo contains a collection of items which were imported using “Import from Excel”. Each item represents a sales record. This data, and more 100% copyright free test data, is offered [here](https://excelbianalytics.com/wp/downloads-18-sample-csv-files-data-sets-for-testing-sales/).

PACoCo uses only a portion of a 50.000 sales record set and well data that complies to:
- Region = Europe
- Country = The Netherlands

## Functionalities

This section gives a high-level overview of the functionalities in the companion canvas app PACoCo:

- When a user starts PACoCo, the code in the button "btn_Start" is executed. It contains code that needs to be run only once per app start.
- Then, the user is navigated to the screen "Home Screen". The global variable "glb_Redirect" - which is defined in App.OnStart - is used for this.
- The home screen is a screen without any data. This way, the canvas app is opened fast and the user can decide her-/himself which navigation menu item to go to.
- The image shown above is a screenshot of the second screen.
- When a user clicks on a navigation item, (s)he is navigated to the related screen.
- The first screen and the second screen differ in the following points:
  - The first screen uses navigation component PACo_Nav_A (as the home screen does) and the second screen uses navigation component PACo_Nav_B.
  - The second screen uses the component "PACo_DetailsList_A" where the first screen does not use a component for the details list. This is done for testing performance. The details list is by far the most complex component. The first screen has a slightly better performance when using larger data sets.
    - The first screen contains a few extra hidden buttons to simulate the behavior properties of the component "PACo_DetailsList_A".
  - The second screen has a "Select all" checkbox in the header. The first screen not.
- The items in the command bar depend on the amount of selected items (0, 1 or more than 1).
  - New > Add a new item
  - Edit > Edit the selected item
  - Delete > Delete the selected item. A dialog box is shown first.
  - Reload > The screen is reloaded. A dialog box is shown first.
    - A redirection screen is used to accomplish this.
- Header columns have been configured for sorting.
  - A user can click the header again to change the sorting (Ascending, Descending).
  - You can configure which column can be used for sorting.
  - Only one column can be used for sorting.
- The width of a header column is fixed but can be configured.
- When the total width of the columns is more wide than the available space, a horizontal scrollbar is shown.
- The items shown in the details list can be filtered with the seach box. The column used for filtering is shown in the hint text.
  - Multiple columns can be used for filtering if needed.
- When an item is clicked on, a panel is shown containing all properties to show.
  - The panel has an edit and delete command which is related to the same commands in the command bar.
- The header in the home screen contains a help icon which open the webpage: https://github.com/formsandflows/PACo/
- The header in the home screen contains a settings icon to show the settings menu.
- The settings menu has two items: Themes and Languages
- The setting "Themes" navigates a user to the themes screen from where a theme can be selected: Default, Dark, High-contract or Fluent UI
- The setting "Languages" navigates a user to the languages screen from where a language can be selectd: English, Dutch
- The header of the themes and languages screen contains a back icon to navigate back to the home screen.

## Responsiveness

PACoCo is a responsive app with the following setup:

- The minimum width of a screen is 1024. When the screen width is less, a horizontal scrollbar is shown.
- There is no maximum width for a screen. The app has a maximum width of 1800 though. This means that when a screen width is larger than 1800, the app width is 1800 and shown horizontal centered.
- The minum height of a screen is 640. When the screen height is less, a vertical scrollbar (and therefor also a horizontal scrollbar) is shown .

## Screens
There are four special screens in PACoCo which need some extra explanation:

- Color Screen
- Controls Screen
- Redirect Screen
- Start Screen

The other screens are accessible when running the canvas app.

### Color screen
This screen is only visible in edit mode and it contains a block per palette slot. See [Theming](./theming.md) for more information on palette slots. A block contains the name of the palette slot and its related color code. The color of the text is set to its color property. The actual values depend on the active theme. For example, theme "Default" will show:

![image](https://user-images.githubusercontent.com/35654198/235985325-25614c97-c027-492e-bd56-579446bb5730.png)

### Controls screen
This screen is only visible in edit mode and contains default controls which are configured to work with the theming setup of PACo. These controls can for instance be used on a custom form.

![image](https://user-images.githubusercontent.com/35654198/235985418-04c6887b-88ee-470b-aadb-585f6cfe4da4.png)

### Redirect screen
The navigation has the following setup:

1. Each navigation item (menu item) is related to a dedicated screen.
2. When a navigation item is clicked on, the current screen is configured in the global variable "glb_RedirectScreen".
3. The user is then navigated to the screen “Redirect Screen”.
4. The property "Onvisible" of the redirect screen has one line of code which selects the button "btn_Redirect".
5. The property "OnSelect" of the button "btn_Redirect" has code to redirect the logged in user to the screen set in the global variable "glb_RedirectScreen".

With this setup, the code in the property "OnVisible" is run again of the navigation item which was clicked on. You can implement your own setup on how to deal with the navigation of course.

The following blog post gives more input: [Run your screen’s "OnVisible" code again with a redirect screen](https://www.formsandflows.nl/2022/08/27/run-your-screens-onvisible-code-again-with-a-redirect-screen/)

To be able to change the code in the property "OnSelect" of the button "btn_Redirect", one line of code is added to the property "OnStart" of the "App" object:

`Set(glb_Redirect, true)`

When setting this global variable to false and then running App.OnStart, the user is not redirected back to the screen in the global variable "glb_RedirectScreen" and the code in button "btn_Start" can be changed to your liking.

### Start screen
The start screen is the first screen used when the app is started. The property "Onvisible" of the start screen has one line of code which selects the button "btn_Start". The property "OnSelect" of the button "btn_Start" has code which needs to be run only once. At the end of the code, the user is navigated to the home screen.

With this setup, the user starting the app sees a spinner as soon as possible.

To be able to change the code in the property "OnSelect" of the button "btn_Start", one line of code is added to the property "OnStart" of the "App" object:

`Set(glb_Redirect, true)`

When setting this global variable to false and then running App.OnStart, the user is not navigated to the home screen and the code in button "btn_Start" can be changed to your liking.
