## Create a Top 5 list

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
In this step, you will create a top 5 ordered list to show the most used emoji.
</div>
<div>
<iframe src="https://trinket.io/embed/html/3fc9fca766?outputOnly=true" width="500" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>
</div>
</div>

--- task ---

Open the [starter project](https://trinket.io/embed/html/769dc6ee61){:target="_blank"}.

--- /task ---

--- task ---

Collapse the `<head>` section to make your code easier to read.

![A short animation demonstrating the mouse clicking on the little triangle next to the line 3 number to collapse the head code.](images/collapse.gif)

--- /task ---

--- task ---

**Look:** at the `<header>` code.

Note that the classes for the header have already been added for you. These set the secondary colours and the bottom border, just like in the [Anime expressions](https://projects.raspberrypi.org/en/projects/anime-expressions){:target="_blank"} project.

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 30
line_highlights: 30
---
  <header class="secondary border-bottom">

  </header>

--- /code ---

--- /task ---

--- task ---

Add an `<h1>` heading with the content `Top 5 Emoji!`.

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 30
line_highlights: 31
---
  <header class="secondary border-bottom">
    <h1>Top 5 Emoji!</h1>

--- /code ---

--- /task ---

--- task ---

Within your `<main>` tags, add in `<section>` tags for your Top 5 emoji list. Remember to leave a blank line between the `<section>` tags to give you room to add more content. 

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 34
line_highlights: 35-37
---
    <main>
      <section>
       
      </section>

    </main>

--- /code ---

--- /task ---

Lists are a great way to display information on a webpage. A list contains multiple list items `<li>`. There are two types of list:

+ An **unordered list** `<ul>` is where each new item starts with a bullet point. An unordered list could be ingredients on a shopping list or your favourite colours.
+ An **ordered list** `<ol>` is where each new item is numbered and the order written is important. A use for an ordered list could be a top ten songs list or a sports league table.

Can you think of another use for an unordered list and an ordered list?

--- task ---

Within your `<section>` tags, add in `<ol>` tags to create an ordered list. 

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 34
line_highlights: 36-38
---
    <main>
      <section>
        <ol>

        </ol>
      </section>

    </main>

--- /code ---

--- /task ---

--- task ---

Within your `<ol>` tags, add in an `<li>` tag for your first item in the list. This includes the `rolling on the floor emoji` 🤣. To get the emoji icon you can **copy and paste** it from below or use the emoji keyboard.

--- collapse ---
---
title: Use the emoji keyboard
---

Keyboard shortcuts can be used to access the emoji keyboard on your computer. Below are common keyboard shortcuts:

**Windows**

Select Windows and press the dot '.' (full stop or period) at the same time.

**Linux**

Select Ctrl + Alt + E together.

**Mac**

Select CTRL + CMD + Space together.

--- /collapse ---

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 34
line_highlights: 37
---
    <main>
      <section>
        <ol>
          <li>🤣 – Rolling on the floor laughing.</li>
        </ol>
      </section>

    </main>

--- /code ---

Note that your emoji will look different on different operating systems. 

--- /task ---

--- task ---

Add the code for the remaining list items `<li>`. 

👍👍🏻👍🏼👍🏽👍🏾👍🏿 Some emoji, for example thumbs up and folded hands, have multiple skin tones to choose from. You can add one or include all of the options in your list. 

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 34
line_highlights: 38-41
---
    <main>
      <section>
        <ol>
          <li>🤣 – Rolling on the floor laughing.</li>
          <li>👍👍🏻👍🏼👍🏽👍🏾👍🏿 – Thumbs up.</li>
          <li>😭 – Loudly crying face.</li>
          <li>🙏🙏🏻🙏🏽🙏🏽🙏🏾🙏🏿 – Folded hands.</li>
          <li>😘 – Face blowing a kiss.</li>
        </ol>
      </section>

    </main>

--- /code ---

--- /task ---

--- task ---

**Test:** Check that your output shows a numbered list. The web browser inserts the numbers for you so it's easy to add and remove list items. 

**Tip:** If your computer doesn't support emoji then you can make them from characters such as ';)'.

<iframe src="https://trinket.io/embed/html/3fc9fca766?outputOnly=true" width="600" height="500" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>

--- /task ---