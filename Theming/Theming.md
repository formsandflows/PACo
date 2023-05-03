# Theming

Theming is based on the way how theming is implemented in [Fluent UI](https://developer.microsoft.com/fluentui/) using palette slots with something extra: Each palette slot also has a color property containing a hex color code. These color properties are used for text colors. Example: When a button uses a certain palette slot for the property "Fill", the property "Color" has the value set in the related color property. This makes sure that text is readable.

The canvas components have a theme configuered which is based on the default Fluent UI theme. This theme is called "Fluent UI". All components have a property "cmp_Theme" with with the configured theme can be overruled. The companion canvas app [PACoCo](.//PACoCo.md) includes three extra themes:

- Default
- Dark
- High-contrast

All four themes have their own file in this repository.

PACo does not use all palette slots.

The companion canvas app [PACoCo](.//PACoCo.md) contains a screen (Color Screen) which is only visible in edit mode containing a block for each palette slot of the current active theme. Example from theme "Default":

![image](https://user-images.githubusercontent.com/35654198/235984971-b88b94e3-d379-4b98-bac5-9dc9cacd0bb5.png)

This color screen can help you in creating your own themes.
