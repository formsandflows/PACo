# Theming

**Soon, a new major version (Version 3.0) will be released. This documentation is related to that version and is still "Under construction"!**

Theming is based on the way how theming is implemented in [Fluent UI](https://developer.microsoft.com/fluentui/) by using palette slots with something extra: Each palette slot also has a related color property containing a hex color code which has a good contrast with its related palette slot. These additional color properties make is much easier to work with colors in PACo canvas components.

Below is an example of the property "Color" of the text label control used in the PACo canvas component "PACo_Button_A":

![image](https://github.com/formsandflows/PACo/assets/35654198/fa7ce3ba-43ac-44e0-8b72-c215ef737ffd)

All PACo canvas components have a custom property called "cmp_Theme" which contains the default theme. **Because of this setup, you can define your own theme in the canvas app using the PACo canvas components.**

There are a few canvas components who have custom properties which contain also a color related property. These properties overrule the theme.

The companion canvas app [PACoCo](.//PACoCo.md) includes three themes:
- Default
- Dark
- High-contrast

All three themes have their own file in this repository.

PACo does not use all palette slots. Only the following palette slots are used:
- black
- neutralLighter
- neutralTertiary
- themePrimary
- white

The companion canvas app [PACoCo](.//PACoCo.md) uses some addition the palette slots.

The companion canvas app [PACoCo](.//PACoCo.md) contains a screen (Color Screen) which is only visible in edit mode containing a block for each palette slot of the current active theme. The text in the block has a color as defined in the related color property. Example from theme "Default":

![image](https://user-images.githubusercontent.com/35654198/235984971-b88b94e3-d379-4b98-bac5-9dc9cacd0bb5.png)

This color screen can help you in creating your own themes.
