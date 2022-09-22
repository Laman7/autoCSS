# AutoCSS (v1.4)

1. Addition of 6 colors (Off colors and Shades of Grey)
2. Font sizes to match perfect fifth (based on type-scale.com)

# Auto CSS (v1.3)

## To make development quicker and easier for developer.
Systematic approach to web development instead of manually adding padding, margin and sizing.

## Break Points - Conditions
- Designed to fit 1400px screen 
- Full 12 grid size 1312px with 80px Column and 32px Gutter; Total is 112px per Column.
- Break even point
- Desktop: 1312px (-xl)
- Tablet: 992px (-lg)
- Landscape: 768px (-md)
- Portrait/Mobile: 480px (-sm)

## Steps
1. Get color code from Mycolorspace (https://mycolor.space/)
2. Change the variable in line 26-47
3. Load the CSS first before style.css


# New in 1.3
- Grid systems
- Improvement on .btn, adding btn-white

## Grid
New grid system adds easier to code from design.

CSS | Grid Behavior
--- | --- 
.grid-2 |  Creates 2 columns
.grid-3 |  Creates 3 columns
.grid-4 |  Creates 4 columns
.grid-5 |  Creates 5 columns
.grid-1-2 |  Creates 1 then 2 spacing (2 columns)
.grid-1-3 |  Creates 1 then 3 spacing (2 columns)
.grid-2-1 |  Creates 2 then 1 spacing (2 columns)
.grid-2-3 |  Creates 2 then 3 spacing (2 columns)
.grid-3-1 |  Creates 3 then 1 spacing (2 columns)
.grid-3-2 |  Creates 3 then 2 spacing (2 columns)
.grid-xl-reverse ,.grid-lg-reverse |  Reverse the order in 992px size. Apply to child grid.
.grid-l-reverse ,.grid-md-reverse |  Reverse the order in 768px size. Apply to child grid.
.grid-m-reverse ,.grid-sm-reverse |  Reverse the order in 480px size. Apply to child grid.

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
.primary-off | change color to primary
.secondary | change color to secondary
.secondary-off | change color to secondary
.accent | change color to accent
.accent-off | change color to accent
.base | change color to base

### Colors Explained
Primary | it should be the color you want people to remember you by
Secondary | complementing colors the primary
Accent | Complete opposite to the primary colors
Base | The main website background color
Grey | Use as logically possible
Body | Main text color
Body Off | Use it for lesser importance


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
.width-xs, .width-2 | Size of 2 columns, 192px
.width-s, .width-25, .width-3 | Size of 3 columns, 304px (25%)
.width-m, .width-4 | Size of 4 columns, 448px
.width-l, width-50 ,.width-6| Size of 6 columns, 640px (50%)
.width-xl, .width-8 | Size of 8 columns, 864px
.width-xxl, .width-10 | Size of 10 columns, 1088px
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

### Remove Padding at Breakpoint 
Remove the padding at certain breakpoint

CSS | What it does 
--- | --- 
.pad-l-0, .pad-xl-0, .pad-xl-none | Removes padding at 1312px
.pad-m-0, .pad-lg-0, .pad-lg-none | Removes padding at 992px
.pad-md-none, .pad-l-none, .pad-md-0  | Removes padding at 768px
.pad-sm-none, .pad-m-none, .pad-sm-0 | Removes padding at 480px

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
.center-h | centers element to horizontal
.center-v | centers element to vertical
.center-self | applies margin auto

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