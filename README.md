# Lesson Task: CSS Box Model, Floats, Positioning, Transitions
## 1. Setup
Keep using your 3-page site (index.html, about.html, contact.html).
All CSS should go in your shared styles.css.
Remove old inline styles if any.

### Tips

Minimal HTML tweaks you should add:
* Put `id="top"` on the first element in each page (e.g., `<body id="top">` or the main `<h1>`).
* Add a fixed “Back to Top” link: `<a href="#top" id="to-top" class="btn">Top</a>` (place it near the end of `<body>`).
* For the *About* page float demo, create three boxes: `<div class="float-grid"><div class="float-box">1</div><div class="float-box">2</div><div class="float-box">3</div></div><p class="clearfix"></p>`
(or add `.clearfix` to the element right after the float boxes)

## 2. Tasks
### Task A – Borders
* On **index.html**, add a border around your main content area:
    * Use border: `2px solid darkblue;`.
* On **about.html**, style the table so each cell has `1px solid gray` borders.
* On **contact.html**, make the form inputs have `2px dashed green` borders when focused (`input:focus`).

### Task B – Margins
* Add spacing between sections with `margin-bottom: 30px;`.
* On **index.html**, make all list items have `margin-bottom: 5px;`.
* Experiment with margin collapse:
    * Add two `<p>` tags in a row and give them top/bottom margins.
    * Observe how the margins collapse in the Web Inspector.

### Task C – Paddings
* On **index.html**, add padding inside the main content area (`padding: 20px;`).
* On **about.html**, give table headers (th) extra padding (`padding: 10px;`).
* On **contact.html**, make buttons have more clickable space with `padding: 12px 20px;`.


### Task D – Floating
* On **index.html**, float an image to the left of some text.
* Add margin to the image so text doesn’t stick to it (`margin: 0 10px 10px 0;`).
* On **about.html**, create 3 small colored boxes (`div`s) floated left, each `width: 100px; height: 100px;`.
* Use `clear: both;` after them so following text isn’t overlapped.


### Task E – Positioning
* On **index.html**, make a “Back to Top” button that is **fixed** at the bottom-right of the screen.
* On **about.html**, use **absolute positioning** to place a label in the top-right corner of the table (e.g., “Table 1”).
* On **contact.html**, make the header **sticky** at the top of the page 
(`position: sticky; top: 0;`).


### Task F – Transitions
* On **index.html**, add a hover transition to navigation links:
    * `transition: color 0.3s ease;`
    * Change text color smoothly on hover.
* On **about.html**, make the floated boxes grow slightly on hover using 
`transform: scale(1.05);` `transition: transform 0.2s ease-in-out;`.
* On **contact.html**, make the submit button smoothly change background color when hovered.


### Check with DevTools (Web Inspector):
* Inspect main to see **border + padding** in the Box Model.
* Inspect two adjacent `<p>` elements to see **margin collapse**.
* Inspect the floated image (`.float-left`) and float boxes (`.float-box`) to see how surrounding content flows and how clearfix contains floats.
* Scroll and watch the **fixed** “Top” button and **sticky** header behavior.
* Hover nav links, float boxes, and the submit button to see **transitions** in action.
