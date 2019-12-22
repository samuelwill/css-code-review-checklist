## CSS Code Review Checklist

### Principles
1. <b>Specificity</b> should be kept as <b>low</b> as possible
2. Styling code should be <b>generic</b> and reusable across components and projects
3. Separate <b>structure</b> from <b>skin</b>. Classes should manage the layout or look of an element, not both

### Checklist
- [ ] The developer understands our `ITCSS` architecture and has extended the system in the correct places
- [ ] All CSS code is written using a <b>preprocessor</b> like <i>SCSS</i> or <i>LESS</i>
- [ ] All CSS is run through a <b>postprocessor</b> like <i>Webpack</i> for concatenation, minification, vendor prefixing, etc
- [ ] All styles are applied using <b>classes</b> that follow the <b>BEM</b> naming convention
- [ ] `#ids` and elements (like `p` or `div`) are not used to apply styling
- [ ] No `!important`s are used outside of override classes
- [ ] Developer has confirmed with UX the need for any <b>responsive styling</b>
- [ ] Only `rem` units are used, not `px` or `em`s
- [ ] No inline styles are used
- [ ] `Flexbox` or `Grid` are used to achieve layouts, not floats, tables or Javascript
- [ ] Colors are defined using <b>variables</b> and given a clear name
- [ ] `media queries` are defined inside the associated BEM class definitions
- [ ] All styles are defined <b>mobile-first</b> (media queries apply to progressively larger viewports)
- [ ] No nested selectors are used
