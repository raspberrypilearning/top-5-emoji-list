## Animate more emoji

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">

In this step you will add animated emoji to your website header.

</div>
<div>
<iframe src="https://trinket.io/embed/html/bab7a842c9?outputOnly=true" width="500" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>
</div>
</div>

You have made your website header engaging by using bold colours and a stylish font. Header animations will make the website really eye-catching.

--- task ---

Add 5 emoji to your header, use the `bigfont` class to make them large. 

The `<span>` tag will allow you to add different animations to each emoji later.

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

--- /task ---


--- task ---

Click on the `animation.css` file and find the `bounceme` class. 

The `bounce` animation runs with `ease` timing so the animation starts and ends slowly but speeds up in the middle. 

To create a bounce effect the `scale` property adjusts the size and the `translateY` property moves the element up and down the Y-axis. 

--- code ---
---
language: css
filename: animation.css
line_number_start: 16
line_highlights: 16-19
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

--- /task ---

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

**Debug:**

--- collapse ---

---
title: An emoji in the list is bouncing instead of one in the header!
---

You need to add `bounceme` to an emoji in the `<header>` not the emoji in the `<ol>`. 


--- /collapse ---

--- /task ---

When you look at a webpage, the part that is visible to you is called the **viewport**. A mobile phone will have a much smaller viewport than a desktop computer screen.

Your project already has code to control the **viewport** size and scale to adapt to the device width. You can use viewport in animations to make the animation change to fit the viewport.  

--- task ---

Click on the `animation.css` file and find the `rotatemeleft` class. A combination of `translate` and `rotate` is used to create the roll. 

This `translate` code uses `vw` (viewport-width). The start point of `-60vw` is 60% left of the coded position on the viewport. The animation ends in the coded position `0vw`. 

--- code ---
---
language: css
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

**Test:** Your rolling on the floor laughing emoji 🤣 should move in from the left rotating as it moves. 

--- /task ---

--- task ---

**Choose:** Add animation classes to the remaining emoji 😇😭😘 to finish your fun, eye-catching header. 

You can use any animations from the `animation.css` file:
+ spinme
+ bounceme
+ scaleme
+ rollmeleft
+ rollmeright

<div>
<iframe src="https://trinket.io/embed/html/f47b6c786e?outputOnly=true" width="500" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>
</div>

--- /task ---
