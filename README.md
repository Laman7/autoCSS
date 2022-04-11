*,::after,::before{box-sizing:border-box}
body{min-height:100vh; text-rendering:optimizeSpeed}
img,picture{max-width:100%}
button,input,select, textarea{font:inherit}
@media (prefers-reduced-motion: reduce) {
    html:focus-within {
        scroll-behavior: auto;
    }
    *,
    *::before,
    *::after {
        -webkit-animation-duration: 0.01ms !important;
        animation-duration: 0.01ms !important;
        -webkit-animation-iteration-count: 1 !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.01ms !important;
        scroll-behavior: auto !important;
    }
}
:focus,button:focus{outline-offset:.5rem;outline:var(--primary) solid .2rem}
:focus:not(:focus-visible),button:focus:not(:focus-visible){outline-offset:.5rem;outline:var(--primary) solid .2rem}
:-moz-focus-inner{outline:.2rem solid var(--primary)!important;outline-offset:.5rem}
:focus:not(:focus-visible){outline:0}

:root {
    --primary: #4285F4;
    --secondary: #00257E;
    --accent: #C8A762;
    --base: #E6F4F1;
    --white: #fff;
    --black: #111;
    --body-color: #111;
    --body-mute: #333;
    --grey: #ededed;
    --hover-brightness: 1.3;
    --border-radius: 0.5rem;
    --xxxl: 7rem        /*112px*/;
    --xxl: 5rem         /*80px*/;
    --xl: 3rem          /*48px*/;
    --l: 2rem           /*32px*/;
    --m: 1.5rem         /*24px*/;
    --body: 1.125rem    /*18px*/;
    --s: 1rem          /*16px*/;
    --xs:0.75rem         /*12px*/;
    --lh-heading: 1em;
    --lh-body: 1.5em;
	--ls-heading:-0.025em;

    --clamp-xs: clamp(0.625rem, calc(0.625rem + ((1vw - 0.3rem) * 0.2404)), var(--xs));
    --clamp-s: clamp(0.875rem, calc(0.875rem + ((1vw - 0.3rem) * 0.2404)), var(--s));
    --clamp-m: clamp(1.125rem, calc(1.125rem + ((1vw - 0.3rem) * 0.7212)), var(--m));
    --clamp-l: clamp(1.5rem, calc(1.5rem + ((1vw - 0.3rem) * 0.9615)), var(--l));
    --clamp-xl: clamp(1.75rem, calc(1.75rem + ((1vw - 0.3rem) * 2.4038)), var(--xl));
    --clamp-xxl: clamp(2.5rem, calc(2.5rem + ((1vw - 0.3rem) * 4.8077)), var(--xxl));
    --clamp-xxxl: clamp(3rem, calc(3rem + ((1vw - 0.3rem) * 7.6923)), var(--xxxl));
    --clamp-body: clamp(1rem, calc(1rem + ((1vw - 0.3rem) * 0.2404)), var(--body));
    --width-card: 26rem;
    --width-card-m: 40rem;
    --width-card-l: 54rem;
    --width-content: 1080px;

}

/*Typography*/
html{
    background-color: --base;
}
body {
    font-size: var(--body);
    font-size: var(--clamp-body);
    color: var(--body-color);
    line-height: var(--lh-body);
    background-color: var(--base);
}
.text-xxxl {
    font-size: var(--xxxl);
    font-size: var(--clamp-xxxl);
}
h1, .text-xxl {
    font-size: var(--xxl);
    font-size: var(--clamp-xxl);
}
h2, .text-xl{
    font-size: var(--xl);
    font-size: var(--clamp-xl);
}
h3, .text-l {
    font-size: var(--l);
    font-size: var(--clamp-l);
}
h4, .text-m {
    font-size: var(--m);
    font-size: var(--clamp-m);
}
h5, h6, .text-s {
    font-size: var(--s);
    font-size: var(--clamp-s);
}
.text-xs{
    font-size: var(--xs);
    font-size: var(--clamp-xs);
}
h1,h2,h3 {line-height: var(--lh-heading); letter-spacing: var(--ls-heading);}

/* Text */
.text-larger {font-size: 2em;}
.text-smaller {font-size: 0.875em;}

.text-lighter {
    font-weight: 100;
}
.text-light {
    font-weight: 200;
}
.text-bold {
    font-weight: 700;
}
.text-bolder {
    font-weight: 900;
}
.text-italic {
    font-style: italic;
}
.text-oblique {
    font-style: oblique;
}
.text-decoration-none {
    -webkit-text-decoration: none;
    text-decoration: none;
}
.text-underline {
    -webkit-text-decoration: underline;
    text-decoration: underline;
}
.text-underline-wavy {
    -webkit-text-decoration: underline wavy;
    text-decoration: underline wavy;
}
.text-underline-dotted {
    -webkit-text-decoration: underline dotted;
    text-decoration: underline dotted;
}
.text-underline-double {
    -webkit-text-decoration: underline double;
    text-decoration: underline double;
}
.text-underline-dashed {
    -webkit-text-decoration: underline dashed;
    text-decoration: underline dashed;
}
.text-overline {
    -webkit-text-decoration: overline;
    text-decoration: overline;
}
.text-line-through {
    -webkit-text-decoration: line-through;
    text-decoration: line-through;
}
.text-transform-none {
    text-transform: none;
}
.text-uppercase {
    text-transform: uppercase;
}
.text-lowercase {
    text-transform: lowercase;
}
.text-capitalize {
    text-transform: capitalize;
}
.text-left {
    text-align: left;
}
.text-center {
    text-align: center;
}
.text-right {
    text-align: right;
}
.text-justify {
    text-align: justify;
}
.ct-text-block {padding: 0.5rem 0}
.primary {color: var(--primary)}
.secondary {color: var(--secondary)}
.accent {color: var(--accent)}
.base {color: var(--base)}

/* Space System */

.space-v-s:not(.ct-section) > * + * {
    margin-top: var(--s);
    margin-top: var(--clamp-s);
}
.space-v-m:not(.ct-section) > * + * {
    margin-top: var(--m);
    margin-top: var(--clamp-m);
}
.space-v-l:not(.ct-section) > * + * {
    margin-top: var(--l);
    margin-top: var(--clamp-l);
}
.space-v-xl:not(.ct-section) > * + * {
    margin-top: var(--xl);
    margin-top: var(--clamp-xl);
}
.space-h-s:not(.ct-section) > * + * {
    margin-left: var(--s);
    margin-left: var(--clamp-s);
}
.space-h-m:not(.ct-section) > * + * {
    margin-left: var(--m);
    margin-left: var(--clamp-m);
}
.space-h-l:not(.ct-section) > * + * {
    margin-left: var(--l);
    margin-left: var(--clamp-l);
}
.space-h-xl:not(.ct-section) > * + * {
    margin-left: var(--xl);
    margin-left: var(--clamp-xl);
}

section{
    padding: 0 clamp(1rem, calc(1rem + ((1vw - 0.3rem) * -1.9038)), 0.01rem);
}

/* Width System */

.width-xs:not([class*="breakout--"]) {
    width: 100%;
    
    max-width: 22rem;
}
.width-s:not([class*="breakout--"]) {
    width: 100%;
   
    max-width: 26rem;
}
.width-m:not([class*="breakout--"]) {
    width: 100%;
    max-width: 40rem;
}
.width-l:not([class*="breakout--"]) {
    width: 100%;
    /* max-width: calc((128 * 0.6) * 1rem); */
    max-width: 54rem;
}
.width-xl:not([class*="breakout--"]) {
    width: 100%;
    /* max-width: calc((128 * 0.8) * 1rem); */
    max-width: 68rem;
}

.width-vp-max:not([class*="breakout--"]) {
    width: 100%;
    max-width: calc((128 - 3 * 2) * 1rem);
    margin-left: auto;
    margin-right: auto;
}
.width-50:not([class*="breakout--"]) {
    width: 100%;
    max-width: calc((128 / 2) * 1rem);
}
.width-full:not([class*="breakout--"]) {
    width: 100%;
    max-width: 100%;
}
.width-auto {
    width: auto !important;
    width: 100%;
}
.card {
    background-color: var(--white);
    box-shadow: rgba(0, 0, 0, 0.1) 0px 10px 15px -3px, rgba(0, 0, 0, 0.05) 0px 4px 6px -2px;
    margin: 2rem 0;
    border-radius: var(--border-radius);
}

/* Padding */

.pad-xs:not(.ct-section) {
    padding: var(--xs);
    padding: var(--clamp-xs);
}
.pad-s:not(.ct-section) {
    padding: var(--s);
    padding: var(--clamp-s);
}
.pad-m:not(.ct-section) {
    padding: var(--m);
    padding: var(--clamp-m);
}
.pad-l:not(.ct-section) {
    padding: var(--l);
    padding: var(--clamp-l);
}
.pad-xl:not(.ct-section) {
    padding: var(--xl);
    padding: var(--clamp-xl);
}

.pad-v-xs:not(.ct-section) {
    padding: var(--xs) 1.5rem;
    padding: var(--clamp-xs) 1.5rem;
}
.pad-v-s:not(.ct-section) {
    padding: var(--s) 1.5rem;
    padding: var(--clamp-s) 1.5rem;
}
.pad-v-m:not(.ct-section) {
    padding: var(--m) 1.5rem;
    padding: var(--clamp-m) 1.5rem;
}
.pad-v-l:not(.ct-section) {
    padding: var(--l) 1.5rem;
    padding: var(--clamp-l) 1.5rem;
}
.pad-v-xl:not(.ct-section) {
    padding: var(--xl) 1.5rem;
    padding: var(--clamp-xl) 1.5rem;
}
/* 
.pad-h-xs {
    padding: var(--xs) ;
    padding: var(--clamp-xs);
}
.pad-h-s {
    padding: var(--s) ;
    padding: var(--clamp-s);
}
.pad-h-m {
    padding: var(--m) ;
    padding: var(--clamp-m);
}
.pad-h-l {
    padding: var(--l) ;
    padding: var(--clamp-l);
}
.pad-h-xl {
    padding: var(--xl) ;
    padding: var(--clamp-xl);
} */
.section-pad-s{
    padding: 3rem 1.5rem;
    padding: clamp(1rem, calc(1rem + ((1vw - 0.3rem) * 3.8462)), 3rem) 1.5rem;
}
.section-pad-m{
    padding: 6rem 1.5rem;
    padding: clamp(2rem, calc(2rem + ((1vw - 0.3rem) * 7.6923)), 6rem) 1.5rem;
}
.section-pad-l{
    padding: 9rem 1.5rem;
    padding: clamp(3rem, calc(3rem + ((1vw - 0.3rem) * 11.5385)), 9rem) 1.5rem;
}
.section-pad-xl{
    padding: 12rem 1.5rem;
    padding: clamp(4rem, calc(4rem + ((1vw - 0.3rem) * 15.3846)), 12rem) 1.5rem;
}


/* Center */
.center-all:not(.ct-section),
.ct-section.center-all > .ct-section-inner-wrap {
    display: flex;
    flex-direction: column;
    align-items: center;
    align-content: center;
    justify-items: center;
    justify-content: center;
    text-align: center;
}
.center-y:not(.ct-section),
.ct-section.center-y > .ct-section-inner-wrap {
    flex-direction: column;
    justify-items: center;
    justify-content: center;
    align-items: flex-start;
}
.center-x:not(.ct-section),
.ct-section.center-x > .ct-section-inner-wrap {
    display: flex;
    flex-direction: column;
    justify-items: center;
    justify-content: center;
    align-items: center;
}

@media (max-width: 991px) {
    .center-all-l:not(.ct-section),
    .ct-section.center-all-l > .ct-section-inner-wrap {
        display: flex;
        flex-direction: column;
        align-items: center;
        align-content: center;
        justify-items: center;
        justify-content: center;
        text-align: center;
    }
    .center-y-l:not(.ct-section),
    .ct-section.center-y-l > .ct-section-inner-wrap {
        flex-direction: column;
        justify-items: center;
        justify-content: center;
        align-items: flex-start;
    }
    .center-x-l:not(.ct-section),
    .ct-section.center-x-l > .ct-section-inner-wrap {
        display: flex;
        flex-direction: column;
        justify-items: center;
        justify-content: center;
        align-items: center;
    }
}
.center-self {
    margin-left: auto;
    margin-right: auto;
}

.sticky {
    position: -webkit-sticky;
    position: sticky;
    top: 0;
}
.sticky-top-s {
    top: 2.5%;
}
.sticky-top-m {
    top: 5%;
}
.sticky-top-l {
    top: 10%;
}

/* Button */

.btn-primary {
    background-color: var(--primary);
    border: 0.125em solid var(--primary);
    padding: 1em 1.5em;
    border-radius: 30rem;
    font-size: var(--body);
    font-size: var(--clamp-body);
}
.btn-primary.btn-outline {
    background-color: transparent;
    color: var(--primary);
}

.btn-secondary {
    background-color: var(--secondary);
    border: 0.125em solid var(--secondary);
    padding: 1em 1.5em;
    border-radius: 30rem;
    font-size: var(--body);
    font-size: var(--clamp-body);
}
.btn-secondary.btn-outline {
    background-color: transparent;
    color: var(--secondary);
}
.btn-accent {
    background-color: var(--accent);
    border: 0.125em solid var(--accent);
    padding: 1em 1.5em;
    border-radius: 30rem;
    font-size: var(--body);
    font-size: var(--clamp-body);
}
.btn-accent.btn-outline {
    background-color: transparent;
    color: var(--accent);
}
.btn-xs {
    font-size: var(--xs);
    font-size: var(--clamp-xs);
    padding: .5em 1em;
    cursor: pointer;
}
.btn-s {
    font-size: var(--s);
    font-size: var(--clamp-s);
    padding: 1em 1.5em;
    cursor: pointer;
}
.btn-m {
    font-size: var(--m);
    font-size: var(--clamp-m);
    padding: 1em 1.5em;
    cursor: pointer;
}
.btn-l {
    font-size: var(--l);
    font-size: var(--clamp-l);
    padding: 1em 1.5em;
    cursor: pointer;
}
.btn-box {
    border-radius: 0.5em;
}

a[class*="btn--"] {
    display: inline-block;
}
.btn-clear {
    background: none;
    border: none;
}

a {
    transition: all 0.5s;
    color: var(--primary);
}
a:hover {
    filter: brightness(var(--hover-brightness));
    text-decoration: underline;
}
button:hover {
    cursor: pointer;
    filter: brightness(var(--hover-brightness));
}
.link-primary {color: var(--primary)}
.link-secondary {color: var(--secondary)}
.link-accent {color: var(--accent)}
.rounded-xs {
    border-radius: 0.4444444444rem;
}
.rounded-s {
    border-radius: 0.25rem;
}
.rounded-m {
    border-radius: 0.5rem;
}
.rounded-l {
    border-radius: 1rem;
}
.rounded-xl {
    border-radius: 2rem;
}
.rounded-xxl {
    border-radius: 4rem;
}
.rounded-circle {
    border-radius: 50%;
}


/* Tables */
table {
    border: 1px solid var(--grey);
    border-radius: var(--border-radius);
    border-spacing: 0;
    display: inline-block;
    max-width: 100%;
    overflow-x: auto;
    padding: 0;
    white-space: nowrap;
}

table td,
table th,
table tr {
    padding: 0.75rem 1rem;
}

table thead {
    background-color: var(--primary);
    border-collapse: collapse;
    border-radius: var(--border-radius);
    color: var(--base);
    border-color: var(--primary);
    margin: 0;
    padding: 0;
}
table thead th:first-child {
    border-top-left-radius: var(--border-radius);
}
table thead th:last-child {
    border-top-right-radius: var(--border-radius);
}
table tr:nth-child(even) {
    background-color: var(--grey);
}

/* Quotes */

blockquote p::before {
    content: open-quote;
    font-size: 2em;
    position: relative;
	top:.125em;
	right:.5em;
	display:block;
	line-height:0;
}

blockquote {
    font-size: var(--m);
    font-size: var(--clamp-m);
    line-height: var(--lh-body);
    margin: 1rem auto;
    max-width: 50vw;
    padding: 1.5rem 1.5rem 1.5rem 2.5rem;
}

blockquote footer {
    color: var(--body-mute);
    font-size: var(--xs);
    font-size: var(--clamp-xs);
    line-height: var(--lh-body);
    padding: 1.5rem 0;
}
ol li,
ul li {
    padding: 0.5rem 0;
}

p {
    margin: 1rem 0;
    padding: 0;
}

pre {
    margin: 1rem 0;
    max-width: var(--width-card-l);
    padding: 1rem 0;
}

pre code,
pre samp {
    display: block;
    max-width: var(--width-card-l);
    padding: 0.5rem 2rem;
    white-space: pre-wrap;
}

form {
    display: block;
    padding: 1.5rem;
}

form header {
    margin: 1.5rem 0;
    padding: 1.5rem 0;
}

input,
label,
select,
textarea {
    display: block;
    font-size: inherit;
}

input[type="checkbox"],
input[type="radio"] {
    display: inline-block;
}

input[type="checkbox"]+label,
input[type="radio"]+label {
    display: inline-block;
    font-weight: normal;
}

input,
select,
textarea {
    border: 1px solid var(--grey);
    border-radius: var(--border-radius);
    margin-bottom: 1rem;
    padding: 0.4rem 0.8rem;
}

input[readonly],
textarea[readonly] {
    background-color: var(--grey);
}

label {
    font-weight: bold;
    margin-bottom: 0.2rem;
}

::selection {
    color: var(--base);
    background: var(--primary);
  }