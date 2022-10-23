# Theming

Theming is based on how theming is implemented for with palette slots in Fluent UI with something additional: Each palette slot also has a color property. These color properties are used for related text colors. Example: When a button uses a certain palette slot for the fill, the related color value is used for the button text. This makes sure that text is good readable.

PACo has a theme included which is based on the default Fluent UI theme. This theme is called "Fluent UI". The companion app PACoCo includes three extra themes:

- Default
- Dark
- High-contrast

All four themes have their own file in this repository.

PACo does not use all palette slots.

The companoin canvas app PACoCo contains a screen (Color Screen) which is only visible in edit mode containing a blok for each palette slot of the current active theme. Example from theme "Default":

![image](https://user-images.githubusercontent.com/35654198/197279296-d19ede43-3529-4df5-a7a8-476d3aa59e30.png)
