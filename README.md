# Auto CSS (v1.1)

## To make development quicker and easier for developer.
Systematic approach to web development instead of manually adding padding, margin and sizing.

### Conditions
- Designed to fit 1400px screen 
- Full 12 grid size 1312px with 80px Column and 32px Gutter; Total is 112px per Column.
- Break even point
- Desktop: 1312px
- Tablet: 992px
- Landscape: 768px
- Portrait: 480px

## Steps
1. Get color code from Mycolorspace (https://mycolor.space/)
2. Change the variable in line 26-47
3. Load the CSS first before style.css

# Font Size

Font size is determined by 16px, 8 pt system and Geometric Pattern. Applied to any text

## Default Font Classes
CSS | Calculated Size
--- | --- 
.text-xxxl |  112px
h1, .text-xxl | 80px
h2, .text-xl | 48px
h3, .text-l | 32px
h4, .text-m | 24px
body |  18px
h5, h6, .text-s | 16px
.text-xs | 12px

h1 h2 h3 default line height: 1em, letter spacing: -0.025


## Text Classes
CSS | what it does 
--- | --- 
.text-larger | current font size x2 
.text-smaller | current font size x 0.875 
.text-lighter | font text weight 100 
.text-light | font text weight 200 
.text-bold | font text weight 700 
.text-bolder | font text weight 900 
.text-italic | font text italic 
.text-oblique | font text oblique 
.text-underline | font text underline
.text-underline-wavy | font text underline 
.text-underline-dotted | font text underline-dotted
.text-underline-double | font text underline-double 
.text-underline-dashed | font text underline-dashed
.text-overline | font text overline 
.text-line-through | font text line-through 
.text-uppercase | font text uppercase 
.text-lowercase | font text lowercase 
.text-capitalize | font text capitalize 
.text-left | font text left 
.text-center | font text center 
.text-right | font text right 
.text-justify | font text justify 
.text-none | font text decoration-none 

## Text Color
CSS | what it does 
--- | --- 
.primary | change color to primary
.secondary | change color to secondary
.accent | change color to accent
.base | change color to base


## Auto Spacing Vertical Elements
Apply at Div. Don't apply it to section. All elements in Div (child) is subjected to space. Similar name: Owl system

CSS | What it does 
--- | --- 
.space-v-s | adds margin top child 16px
.space-v-m | adds margin top child 24px
.space-v-l | adds margin top child 32px
.space-v-xl | adds margin top child 48px

## Auto Spacing Horizontal Elements
Apply at Div. Don't apply to section. All elements in Div (child) is subjected to space. Similar name: Owl system

CSS | What it does 
--- | --- 
.space-h-s | adds margin left child 16px
.space-h-m | adds margin left child 24px
.space-h-l | adds margin left child 32px
.space-h-xl | adds margin left child 48px

## Width and Card
This can be applied to Divs. Based on 12 grid, 112px per column minus 32px
CSS | What it does 
--- | --- 
.width-xs | Size of 2 columns, 192px
.width-s, .width-25 | Size of 3 columns, 304px (25%)
.width-m | Size of 4 columns, 448px
.width-l, width-50| Size of 6 columns, 640px (50%)
.width-xl | Size of 8 columns, 864px
.width-xxl | Size of 10 columns, 1088px
.width-full, .width-100 | 100% full width
.card | looks like card layoout

## Div Padding
### Padding All
This add padding all around div.
CSS | What it does 
--- | --- 
.pad-xs | adds padding all 12px 
.pad-s | adds padding all 16px 
.pad-m | adds padding all 24px 
.pad-l | adds padding all 32px 
.pad-xl | adds padding all 48px 

### Padding Vertical 
This add padding top and bottom. (with default left-right 16px)

CSS | What it does 
--- | --- 
.pad-v-xs | adds padding vertically, top and bottom 12px 
.pad-v-s | adds padding vertically, top and bottom 16px 
.pad-v-m | adds padding vertically, top and bottom 24px 
.pad-v-l,.pad-v | adds padding vertically, top and bottom 32px 
.pad-v-xl | adds padding vertically, top and bottom 48px 

CSS | What it does 
--- | --- 
.pad-h-xs | adds padding horizontally, left and right 12px 
.pad-h-s, .pad-h | adds padding horizontally, left and right 16px 
.pad-h-m | adds padding horizontally, left and right 24px 
.pad-h-l | adds padding horizontally, left and right 32px 
.pad-h-xl | adds padding horizontally, left and right 48px

You can use variable xs, s, m, l, xl, xxl, xxxl or clamp for example
```
#div-box { margin : var(--xs)}
#div-box { margin: var(--clamp-xl)}
```

## Section Padding
CSS | What it does 
--- | --- 
.section-pad-s | adds padding 48px top and bottom
.section-pad-m | adds padding 96px top and bottom
.section-pad-l | adds padding 96px top and bottom
.section-pad-xl | adds padding 192px top and bottom

## Centering
CSS | What it does 
--- | --- 
.center-all | centers everything in container, vertical and horizontal
.center-y | centers element to horizontal
.center-x | centers element to vertical

## 6. Sticky

CSS | What it does 
--- | --- 
.sticky | Stick up
.sticky-top-s | from top 2.5%
.sticky-top-m | from top 5%
.sticky-top-l | from top 10%

## Call to Action
### Button
CSS | What it does 
--- | --- 
.btn-primary | Rounded button with primary color
.btn-secondary | Rounded button with secondary color
.btn-accent | Rounded button with accent color
.btn-outline | Outline rounded button with color
.btn-xs | Button size based on font size 12px
.btn-s | Button size based on font size 16px
.btn-m | Button size based on font size 24px
.btn-l | Button size based on font size 32px

### Link
CSS | What it does 
--- | --- 
Link default color is primary color
.link-primary | Font color primary (just in case)
.link-secondary | Font color is secondary
.link-accent | Font color is accent

### Rounded
CSS | What it does 
--- | --- 
.rounded-s | Border radius of 4px
.rounded-m | Border radius of 8px
.rounded-l | Border radius of 16px
.rounded-xl | Border radius of 32px
.rounded-xxl | Border radius of 64px
.rounded-circle | Border radius of 50%

## Defaults
- Table - Based on MVP
- Blockquote - Based on MVP
- Form - Based on MVP
- ul li ol li - Based on MVP
- Animate – All links are animated