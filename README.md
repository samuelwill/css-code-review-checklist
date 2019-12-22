## CSS Code Review Checklist

### Principles
1. Specificity should always be as low as possible
2. Styling code should be generic and reusable across components and projects
3. Separate structure from skin. Classes should manage the layout or look of an element, not both

### Check List Items
- [ ] The developer understands our `OOCSS` architecture and has extended the system in the correct places
- [ ] All styles are applied using classes that follow the BEM naming convention
- [ ] `#ids` and elements (like `p` or `div`) are not used to apply styling
- [ ] No `!important`s are used outside of override classes
- [ ] Developer has confirmed with UX the need for any responsive styling
- [ ] Only `rem` units are used, not `px` or `em`s
- [ ] No inline styles are used
- [ ] `Flexbox` or `Grid` are used to achieve layouts, not floats, tables or Javascript
- [ ] Colors are defined using variables and given a clear name
- [ ] `media queries` are defined inside the associated BEM class definitions
- [ ] All styles are defined mobile-first. E.g. media queries apply to progressively larger viewports
- [ ] No nested selectors are used
