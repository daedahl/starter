# Flexbox
The flexbox layout aims at providing a  efficient way to distribute intems in a container, even when their size is unknown or dynamic.
## Container Properties
```css
.container {
  display: flex; /* or inline-flex; to make the CONTAINER inline */

  flex-direction: row | column | row-reverse | column-reverse

  flex-wrap: nowrap | wrap | wrap-reverse

  /* This combines direction and wrap */
  flex-flow: column wrap;

  justify-content: flex-start | flex-end | center
                  space-between | space-around | space-evenly

  align-items: flex-start | flex-end | center | stretch | baseline

  align-content: flex-start | flex-end | center
                space-around | space-between | stretch

  /* gap explictly controls space between items only */
  gap: 25px;
  gap: 10px 20px; /* row-gap column-gap */
  row-gap: 15px;
  column-gap: 15px;  
}
```
## Item Properties
```css
.item {
  order: 3; /* default is 0 */

  flex-grow: 3; /* whole number unitless values used as proportions - default is 0*/
  flex-shrink: 1; /* default is 1 */

  /* flex-basis defines a default size */
  flex-basis: auto | 20% | others

  /* Shorthand for flex-grow, flex-shrink, flex-basis */
  flex: 0 1 auto /* default */

  align-self: auto | flex-start | flex-end | center | baseline | stretch;
}
```
## Prefixing
Due to changing specs and browser inconsistancies prefixing is likely needed.
