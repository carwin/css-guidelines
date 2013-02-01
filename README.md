# A Guide To Writing CSS Documents
#### _by Carwin Young_

This is a living guideline I use to enforce stylesheet consistency in my projects.

Typically, my personal projects tend to be quite small - but consistency is key in
any project. Even if you use no indentions and capitalize every other letter, you'll
be better off staying consistent than you will be writing your CSS on a whim.

## CSS declaration order
Rather than arbitrarily ordering declarations on a CSS selector, or alphabetizing
them (also arbitrary), group related declarations together, much like you would group
your SASS partials. This grouping order should help make certain properties easier to
find (based on importance) which means we can make changes rapidly.

**Declaration Groups**
  - Positioning
    - position
    - float
    - clear
    - top
    - right
    - bottom
    - left
    - direction
    - z-index
  - Box Model
    - display
    - [(max|min)-]height
    - [(max|min)-]width
    - margin
    - padding
    - border
    - box-sizing
    - vertical-align
    - long-hand forms of the above properties

Other properties should be grouped with like properties in a way that makes sense

  - font-size
  - font-weight

  - background-color
  - background-position

```css
.class {

  /* Positioning */
  float: left;
  width: 100%;

  /* Box Model */
  display: inline-block;
  vertical-align: middle;

  /* Others */
  background-color: #000;
  color: #fff;

}
```
