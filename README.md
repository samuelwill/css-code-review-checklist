## CSS Code Review Checklist

### Principles
1. <b>Specificity</b> should be kept as <b>low</b> as possible
2. Styling code should be <b>generic</b> and reusable across components and projects
3. Separate <b>structure</b> from <b>skin</b>. Rules should manage the layout or look of an element, not both

### General
- [ ] The developer understands our `ITCSS` architecture and has extended the system in the correct places
- [ ] All CSS code is written using a <b>preprocessor</b> like <i>SCSS</i> or <i>LESS</i>
- [ ] All CSS is run through a <b>postprocessor</b> like <i>Webpack</i> for concatenation, minification, vendor prefixing, etc
- [ ] Developer has appropriately leveraged preprocessor functionality like <b>variables</b>, <b>functions</b> and <b>mixins</b>
- [ ] Only `rem` units are used, not `px` or `em`s
- [ ] Developer has confirmed with UX the need for any <b>responsive styling</b>
- [ ] `media queries` are defined inside the associated BEM class definitions
- [ ] All styles are defined <b>mobile-first</b> (media queries only apply to progressively larger viewports)

### Maintenance
- [ ] All rules are applied using <b>classes</b> that follow the <b>BEM</b> naming convention
- [ ] `#id`s and elements (like `p` or `div`) are not used as selectors
- [ ] No inline styles are used
- [ ] Colors are defined using <b>variables</b> and given a clear name
- [ ] No `!important`s are used outside of override classes

### Performance
- [ ] `Flexbox` or `Grid` are used to achieve layouts, not floats, tables or Javascript
- [ ] `DOM` size has been reduced as much as possible
- [ ] No nested selectors are used
- [ ] <b>Animation</b> is achieved using CSS not Javascript where possible
- [ ] Expensive properties are avoided if possible: <i>border-radius</i>, <i>box-shadow</i>, <i>:nth-child</i>, <i>filter</i>, <i>position: fixed</i>, <i>transform</i>, <i>opacity</i>)
- [ ] <b>Unused</b> CSS has been removed
