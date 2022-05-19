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

Add some emoji to your header with the class `
font` s
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



--- /task ---

--- task ---



--- /task ---





![Animated gif showing a line of xs changing through all the colours in the rainbow.](images/rainbow.gif)

--- code ---
---
language: html
---

/* gradually change colours through a full rainbow 
@keyframes change-color {
  0% { color: red;}
  20% { color: orange;}
  40% { color: yellow;}
  60% { color: green;}
  80% { color: blue;}
  100% { color: purple;}
}

--- /code ---