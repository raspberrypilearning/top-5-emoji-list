## Add a background image

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">

Add a colourful emoji background and make the main part of the page transparent so you can see the image through the main content.


<div>
<iframe src="https://editor.raspberrypi.org/en/embed/viewer/top-5-emoji-list-step-4" width="500" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>


The CSS `background-image` property allows you to set an image to be the background for your webpage.

\--- task ---

**Find:** In `style.css`, find the CSS `body` rule and **uncomment** the `background-image` line to set the background image for your webpage.

## --- code ---

language: css
filename: style.css
line_numbers: true
line_number_start: 44
line_highlights: 47
--------------------------------------------------------

/\* add a background image to body \*/

body {
background-image: url('emojis.png'); /\* Uncomment and change filename to add a background image
/_background-repeat: repeat;_/ /\* Make the image repeat _/
/_background-size: cover;_/ /_ Make the image cover the whole container \*/
}

\--- /code ---

\--- /task ---

\--- task ---

**Test:** Click the **Run** button.

You should see the colourful emoji image at the edges of your webpage.

**Tip** You may need to see your output area to view the background image.

**Tip:** If you view your webpage on a mobile phone, rotate the screen into landscape mode.

\--- /task ---

**Opacity** means how difficult it is to see through an object. An opacity of 1 means an HTML element is fully solid and you cannot see through it. An opacity of 0 means that an element is completely transparent.

\--- task ---

**Find:** In the `style.css` file, find the `/* Add a transparent effect */` comment.

## --- code ---

language: css
filename: style.css
line_numbers: true
line_number_start: 93
line_highlights: 93
--------------------------------------------------------

/\* Add a transparent effect \*/

\--- /code ---

\--- /task ---

So far, you have used CSS classes that were created for you. Now you are going to create a new CSS class called `transparent`, which you can use to make the `<main>` HTML element transparent.

An opacity of `0.95` is slightly transparent.

Add the `.transparent` rule below the comment.

\--- task ---

## --- code ---

language: css
filename: style.css
line_numbers: true
line_number_start: 93
line_highlights: 95-97
-----------------------------------------------------------

/\* Add a transparent effect \*/

.transparent {
opacity: 0.95;
}

\--- /code ---

\--- /task ---

You have added a new CSS class, but now you need to use it.

\--- task ---

Add your new `transparent` class to `<main>` in your HTML file.

## --- code ---

language: html
filename: index.html
line_numbers: true
line_number_start: 34
line_highlights: 34
--------------------------------------------------------

<main class="transparent">
  <section class="wrap">    
    <ol class="wide">

\--- /code ---

\--- /task ---

\--- task ---

**Test:** Click the **Run** button.

Check that the main part of your page is slightly transparent.

What happens if you change the `opacity` to `0.50`, `0.75`, or `0.90`? Try different values in your CSS rule and see which you prefer.

<div>
<iframe src="https://editor.raspberrypi.org/en/embed/viewer/top-5-emoji-list-step-4" width="500" height="700" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>

\--- /task ---
