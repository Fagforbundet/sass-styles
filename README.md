# @fagforbundet/design-library

With inspiration from:
- https://thedesignsystem.guide/design-tokens-naming-playbook

The design library should make available the tools needed to reuse the different parts of Fagforbundet's design profile. When making use of the library, one can choose to include everything by using the base index.scss, or one can include specific parts of the library by referencing what's needed.
For most projects, especially those using SCSS, including everything is the best option. // Is it, tho?

## Folder structure
The `styles` folder contains these folders:
 - `abstracts` -> Contains styles and variables for design tokens and other things that normally won't affect anything directly
 - `base` -> Contains a file containing style references for everything one might need when adding the library to a project. Next to this file one can also find some barrel import files for cleanliness
 - `components` -> Contains styles for design components (i.e. checkbox, button, dropdown, etc.)
 - `layouts` -> Contains styles for layouts. These are often containers for different scenarios (i.e. page layouts, grids, misc. containers, etc. (not component specific layouts (i.e. menu-boxes)))
 - `utilities` -> Contains utility styles (i.e. no-scroll, outlines, skeletons, etc.)


## Variables


### Design components
Styles for design components should be made available with classes (i.e. `.ff-checkbox`, `.ff-button`, `.ff-dropdown`, etc.). The class combined with the `ff-` prefix ensures the availability of styles, while also ensuring low probability of hijacking any elements or other styles.


## Fonts
Font files are present in this project for anyone who might need them, but Google Fonts serve them as well.
### HTML
```html
<link href="https://fonts.googleapis.com/css2?family=Source+Sans+Pro:wght@400;600;700&display=swap" rel="stylesheet">
```
### CSS
```css
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+Pro:wght@400;600;700&display=swap');
```

### From library
```css
/* TODO: Font config separate from reset */
```



## TODO
- assets cleanup
