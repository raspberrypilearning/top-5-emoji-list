## Animate an emoji!

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
In this step you will add a large, animated emoji to make your webpage more engaging.
</div>
<div>
<iframe src="https://trinket.io/embed/html/c7f4645ca2?outputOnly=true" width="500" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>
</div>
</div>

--- task ---

Extra visualisations bring your content to life. Use a large trophy emoji to highlight that these are the most popular emoji. 

Add a new paragraph `<p>` to your `<section>` to display the trophy emoji 🏆. 

The `hugefont` class makes the emoji text really big. 

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 35
line_highlights: 43
---
      <section>
        <ol>
          <li>🤣 – Rolling on the floor laughing.</li>
          <li>👍👍🏻👍🏼👍🏽👍🏾👍🏿 – Thumbs up.</li>
          <li>😭 – Loudly crying face.</li>
          <li>🙏🙏🏻🙏🏽🙏🏽🙏🏾🙏🏿 – Folded hands.</li>
          <li>😘 – Face blowing a kiss.</li>
        </ol>
        <p class="hugefont">🏆</p>  
      </section>

--- /code ---

--- /task ---

--- task ---

**Test:** The big trophy emoji will appear underneath the list. 

--- /task ---

--- task ---

Add the `wrap` class to your `<section>`. This will make your website responsive by adjusting the layout to fit the available space. 

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 35
line_highlights: 35
---
      <section class="wrap">   
         <ol>
           <li>🤣 – Rolling on the floor laughing.</li>
           <li>👍👍🏻👍🏼👍🏽👍🏾👍🏿 – Thumbs up.</li>
           <li>😭 – Loudly crying face.</li>
           <li>🙏🙏🏻🙏🏽🙏🏽🙏🏾🙏🏿 – Folded hands.</li>
           <li>😘 – Face blowing a kiss.</li>
         </ol>
         <p class="hugefont">🏆</p>        
      </section>

--- /code ---

--- /task ---

--- task ---

**Test:** Now the trophy will appear next the list if the web page is wide enough. But the list and the trophy have the same width. 

--- /task ---

The style sheet also includes `wide` and `narrow` classes that you can use to change the width of elements. 

+ Add the `wide` class to the `<ol>` tag. 

+ Add the `narrow` class to your trophy emoji paragraph.

--- task ---

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 35
line_highlights: 36, 43
---
    <section class="wrap">   
         <ol class="wide">
           <li>🤣 – Rolling on the floor laughing.</li>
           <li>👍👍🏻👍🏼👍🏽👍🏾👍🏿 – Thumbs up.</li>
           <li>😭 – Loudly crying face.</li>
           <li>🙏🙏🏻🙏🏽🙏🏽🙏🏾🙏🏿 – Folded hands.</li>
           <li>😘 – Face blowing a kiss.</li>
         </ol>
       <p class="hugefont narrow">🏆</p>     
     </section>
 
--- /code ---

--- /task ---

--- task ---

**Test:** The list should be wider. If your web page is wide enough then the trophy will appear to the right. 

--- /task ---

You can also use HTML and CSS to create **animations** that change elements on a web page. 

A CSS `@keyframes` rule can be set to change over time. You can change colour, position, size, rotation and many more properties. 

`@keyframes` control how the element should look when a percentage of the running animation is complete.

--- task ---

**Find:** the `.spinme` class at the top of the `animation.css` file. The `.spinme` class has been created for you, it runs a CSS animation called `rotate-center` that rotates from a start position of 0 degrees and ends at 360 degrees. 

The line `animation: rotate-center linear 8s 2;` tells the class to use the `rotate-center` animation with `linear` timing so that it runs at the same speed all the way through. The animation runs for 8 seconds and repeats twice.

--- code ---
---
language: CSS
filename: animation.css
line_numbers: true
line_number_start: 1
line_highlights: 1-4
---
.spinme {
  animation: rotate-center linear 8s 2; /* Time taken for animation and number of repetitions */
  display: inline-block;
}

@keyframes rotate-center {
/* The spin me animation code */
  0% { /* Rotate from 0 to 360 degrees */
    transform: rotate(0);
  }
  100% {
    transform: rotate(360deg);
  }
}
 
--- /code ---

--- /task ---

--- task ---

Go back to the `index.html` file. Add the **spinme** class to the paragraph containing the trophy. 

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 35
line_highlights: 43
---

<section class="wrap">   
         <ol class="wide">
           <li>🤣 – Rolling on the floor laughing.</li>
           <li>👍👍🏻👍🏼👍🏽👍🏾👍🏿 – Thumbs up.</li>
           <li>😭 – Loudly crying face.</li>
           <li>🙏🙏🏻🙏🏽🙏🏽🙏🏾🙏🏿 – Folded hands.</li>
           <li>😘 – Face blowing a kiss.</li>
         </ol>
       <p class="hugefont narrow spinme">🏆</p>         
 </section>

--- /code ---

--- /task ---

--- task ---

**Test:** Your trophy should spin twice each time your load the page. 

**Tip:** You can click the arrow next to 'Autorun' to reload your web page and see the animation again. 

--- /task ---

--- task ---

Go back to the `animation.css` file.

**Choose:** Change the last two values in the line `animation: rotate-center linear 8s 2;` to customise your animation. What happens if your run the animation longer than 8 seconds? Do you want your animation to run more than twice? 

<iframe src="https://trinket.io/embed/html/c7f4645ca2?outputOnly=true" width="600" height="500" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>

--- /task ---


