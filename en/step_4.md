## Add a background image

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">

This step will add a colourful emoji background and make the main part of the page transparent so you can see the image through the main content. 

</div>
<div>
<iframe src="https://trinket.io/embed/html/dace865226?outputOnly=true" width="390" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>
</div>
</div>

The CSS `background-image` property allows you to set an image to be the background for your web page. 

--- task ---

**Find:** In `style.css` find the CSS `body` rule and **uncomment** the `background-image` line to set the background image for your webpage. 

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 44
line_highlights: 47
---
/* add a background image to body */

body {
  background-image: url('emojis.png'); /* Uncomment and change filename to add a background image
  /*background-repeat: repeat;*/ /* Make the image repeat */
  /*background-size: cover;*/ /* Make the image cover the whole container */
}

--- /code ---

--- /task ---

--- task ---

**Test:** You should see the colourful emoji image at the edges of your web page. 

**Tip:** If you are viewing your web page on a mobile phone try rotating into landscape mode. 

--- /task ---

**Opacity** means how difficult it is to see through an object. An opacity of 1 means an HTML element is fully solid and you cannot see through it. An opacity of 0 means that an element is completely transparent. 

--- task ---

**Find:** In the `style.css` file. Find the `/* Add a transparent effect */` comment. 

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 98
line_highlights: 98
---

/* Add a transparent effect */
 

--- /code ---

--- /task ---

So far you have used CSS classes that were created for you. Now you are going to create a new CSS class called `transparent` which you can use to make the `<main>` HTML element transparent. 

An opacity of `0.95` is slightly transparent. 

Add the `.transparent` rule below the comment:

--- task ---

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 98
line_highlights: 100-102
---

/* Add a transparent effect */
 
.transparent {
 opacity: 0.95;
}

--- /code ---

--- /task ---

You have added a new CSS class, now you need to use it.

--- task ---

Now add your new `transparent` class to `<main>` in your HTML file:

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 40
line_highlights: 42
---

<main class="transparent">
      <section class="wrap">    
        <div class="wide">

--- /code ---

--- /task ---

--- task ---

**Test:** Now the main part of your page should be slightly transparent. 

What happens if you change the `opacity` to `50`, `75` or `90`. Try different values in your CSS rule and see which you prefer. 

<div>
<iframe src="https://trinket.io/embed/html/dace865226?outputOnly=true" width="500" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>
</div>

--- /task ---
