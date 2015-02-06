Goal of this framework

- To document the issues, and solutions
- To provide a standardized list of classes 
- To provide a reusable structure for css
- To provide a list of utility classes
- To enforce constrain
    + 6 font sizes
    + 6 shades of grey
    + 6 colors: 3 main colors + 3 darker version
    + 4 font-weights: light, regular, medium, bold

This framework is built on SASS/Compass. The layout used within this document uses the pureCSS framework

Main problems encountered

- 100% height columns
    + Flexbox

- Absolute center containers
    + abs position

- Centered images in a container
    - display: table + display: table-cell, vertical align

- Font scaling across different screen widths

- variable padding for containers

- arbitrary element attribute: declarative styling for structural stuff, for prototyping

Namespacing

Typography: t

- font-size, font-family, font-weight, color

Spacing: s

- margin, padding
- Rules here affect how far apart one element is separated from another, including the edge of the container

Layout: l

- alternate layout for components
- e.g. display, positioning, floats, overflow
- This affects how the element is arranged/positioned within the content area


Module: none

- Modules are just called by their names, e.g. dropdown, profile, list
- includes:
    + modal
    + list
    + profile
    + slider
    + notifications
    + form
    + tooltip
    


States: is[State] convention

- This includes variations of the same element under different contexts, such as user input, data, media queries
- e.g. button.isPressed, button.isDisabled




- The structure of the page is defined by layouts, e.g. top nav, sidebar, main content area
- Layouts are containers for modules, e.g. the top nav bar can contain an inline list, a dropdown (stacked-list) and a profile module
- modules can contain sub-modules
- modules consists of elements, which 


Order of hierachy (lowest to highest)
- base elements
    + button, a, span, div, h etc...
- elements in context
    + #form button, #sidebar .list-stacked, #profile img
- elements with state
- modules
    + slider, login form
- modules with state e.g. menu that is constrained by media queries
- containers
- layouts

