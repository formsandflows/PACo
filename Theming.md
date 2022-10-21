Theming is based on how theming is implemented for Fluent UI with something additional: Each palette slot has a Color property. These color properties are used for related text colors. Example: When a button uses a certain palette slot for the fill, the related color value is used for the button text. This makes sure that text is good readable.

PACo has a theme included which is based on the default Fluent UI theme. This theme is called "Fluent UI". The companion app PACoCo includes three extra themes:

- Default
- Dark
- High-contrast

All four themes have their own file in this repository.
