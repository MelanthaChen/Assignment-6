## Table of Contents

- [Technologies Used](#technologies-used)
- [Features Implemented](#features-implemented)
  - [CSS Grid Layout](#css-grid-layout)
  - [Flexbox Layout](#flexbox-layout)
  - [SASS/SCSS Features](#sassscss-features)
    - [Variables](#variables)
    - [Custom Properties](#custom-properties)
    - [Nesting](#nesting)
    - [Interpolation](#interpolation)
    - [Placeholder Selectors](#placeholder-selectors)
    - [Mixins](#mixins)
    - [Functions](#functions)
- [File Structure](#file-structure)
- [How to Run the Project](#how-to-run-the-project)

## Technologies Used

- HTML5
- CSS3 (CSS Grid, Flexbox)
- SASS/SCSS

## Features Implemented

### CSS Grid Layout

- **Grid Layout**: The `grid-layout` class is used for the client section to showcase a dynamic 3-column layout with a gap of 20px between elements. This is implemented using CSS Grid to create a uniform and responsive layout.

### Flexbox Layout

- **Flexbox Layout**: Flexbox is used extensively for the `frame-container` class and `nav` elements to center and align items in a flexible manner. Flex properties are applied for horizontal and vertical alignment.

### SASS/SCSS Features

1. **Variables**:

   - Defined in the `variables.scss` file, variables are used to store colors, padding, and other reusable values like `--main-padding` and gradient colors.

2. **Custom Properties**:

   - CSS Custom Properties are defined within the `:root` selector to store padding and transition values, making the code easy to maintain and update.

3. **Nesting**:

   - Nested classes are used throughout SASS files for better readability and to show relationships between elements. For example, in the `.about` class, nested elements are styled within.

4. **Interpolation**:

   - Interpolation is used to dynamically create class names based on variables. For instance, card classes like `.card-#{$card-type}` allow flexible styling for different card types.

5. **Placeholder Selectors**:

   - Placeholder selectors like `%center-content` are used to define common styling, which is extended by classes like `.frame-container` to avoid repetition.

6. **Mixins**:

   - Mixins are created to implement common patterns like gradient backgrounds and center-flex properties. For instance, `@mixin gradient-background` allows reusing gradient styles in multiple elements.

7. **Functions**:
   - Custom SASS functions are defined to manipulate colors dynamically. An example function `darken-color` is used to darken a color value based on input.

### File Structure

The project is organized into different folders for better structure:

```
/styles
  ├── /common
  │     ├── _reset.scss
  │     ├── _functions.scss
  │
  ├── /layout
  │     ├── _placeholder.scss
  │     ├── _nav.scss
  │     ├── _footer.scss
  │     ├── _grid.scss
  │     ├── _header.scss
  │
  ├── /components
  |     ├── _variables.scss
  │     ├── _about.scss
  │     ├── _projects.scss
  │     ├── _price-feature.scss
  │     ├── _pricing.scss
  │     ├── _cta.scss
  │     ├── _reviews.scss
  │
  └── main.scss
```
