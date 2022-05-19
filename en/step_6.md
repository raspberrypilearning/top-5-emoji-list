## Animate more emoji

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">

In this step you will add animated emoji to your website header.

</div>
<div>
<iframe src="https://trinket.io/embed/html/cff6fa893b?outputOnly=true" width="350" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>
</div>
</div>

You have made your website header engaging by using bold colours and a stylish font. Header animations will make the website really eye-catching.

--- task ---

Add 5 emoji to your header with the class `bigfont` to make them large.font` s

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 29
line_highlights: 31-35
---

  <header class="secondary border-bottom">
    <h1>Top 5 Emoji!</h1>
    <span class="bigfont">🤣</span>
    <span class="bigfont">😇</span>
    <span class="bigfont">😭</span>
    <span class="bigfont">🤩</span>
    <span class="bigfont">😘</span>
  </header>

--- /code ---


--- task ---

Click on the `animation.css` file and find the `bounceme` class. 

This code runs the `bounceme` animation with `ease` timing meaning the animation starts and ends slowly but speeds up in the middle. The animation runs for 2 seconds and repeats 3 times.

To create a bounce effect the `scale` property is used to adjust the size and the `translateY` property moves the element vertically up and down the Y-axis. 

--- code ---
---
language: html
filename: animation.css
line_numbers: true
line_number_start: 29
line_highlights: 31-35
---

.bounceme {
    animation: bounce ease 2s 3; /* runs the 'bounce' animation with ease timing (slow start and end) for two seconds. Runs the animation twice. */
    display: inline-block;
}

@keyframes bounce {
    /* The bounce animation code */
    0% {
        transform: scale(1, 1) translateY(0); /* Starting position and actual size */
    }
    10% {
        transform: scale(1.1, 0.9) translateY(0); /* Grow width and shrink height for pre bounce squash effect */
    }
    30% {
        transform: scale(1, 1) translateY(-6rem); /* Return to actual size and move emoji up 100px from current position */
    }
    50% {
        transform: scale(1, 1) translateY(0); /* Move emoji back to starting position */
    }
}

--- /code ---

--- /task ------ /task ---

--- task ---

Click on the `index.html` file and add the `bounceme` class to the star-struck emoji 🤩.

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 29
line_highlights: 34
---

  <header class="secondary border-bottom">
    <h1>Top 5 Emoji!</h1>
    <span class="bigfont">🤣</span>
    <span class="bigfont">😇</span>
    <span class="bigfont">😭</span>
    <span class="bigfont bounceme">🤩</span>
    <span class="bigfont">😘</span>
  </header>

--- /code ---

--- /task ---

--- task ---

**Test:** Your star-struck emoji 🤩 should bounce 3 times each time your load the page. 

**Tip:** You can click the arrow next to 'Autorun' to reload your web page and see the animation again. 

--- /task ---

When you look at a webpage, the part that is visible to you is called the **viewport**. A mobile phone will have a much smaller viewport than a computer screens.

Your project already has code to control the viewport's size and scale to adapt your site to the device width. You can use viewport in animations to make the animation change to fit the viewport.  

--- task ---

Click on the `animation.css` file and find the `rotatemeleft` class. To create a rolling animation, a combination of `translate` and `rotate` is used. 

This `translate` code uses a unit called `vw` (viewport-width). The start point of `-60vw` is 60% percent to the left of the element's coded position on the viewport. The animation ends with the element in its coded position `0vw`. 

--- code ---
---
language: html
filename: animation.css
line_numbers: true
line_number_start: 61
line_highlights: 61-64
---

.rollmeleft {
  animation: rollleft ease 8s 1;
  display: inline-block;
}

@keyframes rollleft {
  /* The roll animation code */
  from {
    transform: translate(-60vw) rotate(0deg);
    transform-origin: center;
  }

  to {
    transform: translate(0vw) rotate(360deg);
    transform-origin: center;
  }
}

--- /code ---

--- /task ---

--- task ---

Click on the `index.html` file and add the `rollmeleft` class to the rolling on the floor laughing emoji 🤣.

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 29
line_highlights: 34
---

  <header class="secondary border-bottom">
    <h1>Top 5 Emoji!</h1>
    <span class="bigfont rollmeleft">🤣</span>
    <span class="bigfont">😇</span>
    <span class="bigfont">😭</span>
    <span class="bigfont bounceme">🤩</span>
    <span class="bigfont">😘</span>
  </header>

--- /code ---

--- /task ---

--- task ---

**Test:** Your rolling on the floor laughing emoji 🤣 should move from the left of the viewport rotating as it moves. 

**Tip:** You can click the arrow next to 'Autorun' to reload your web page and see the animation again. 

--- /task ---

--- task ---

**Choose:** There are still 3 emoji without animations. You can use any animations from the `animation.css` file:
+ spinme
+ bounceme
+ scaleme
+ rollmeleft
+ rollmeright

Add animation classes to the remaining emoji until you are happy that you have a fun, eye-catching header. 

--- /task ---
