## Add quote and link

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">

In this step, you will use three more HTML tags: `<blockquote>` and `<cite>` to include quotations and `<a>` to add links to other webpages. 

</div>
<div>
<iframe src="https://trinket.io/embed/html/4603f442a9?outputOnly=true" width="500" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>
</div>
</div>

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
A <span style="color: #0faeb0">hyperlink</span> is a clickable link to another webpage. Links are usually underlined or otherwise styled to separate them from the rest of the text. 
</p>

In HTML, the `<a>` tag is used to create links: 

+ You put the link text that appears on the webpage inside `<a>` and `</a>` 
+ The `href` attribute provides the web address (usually beginning with 'https:') of the page you want to link to 
+ You can also add `target="_blank"` to make the linked webpage open in a new tab in the web browser, instead of the new page replacing the current webpage  

--- task ---

We have created a short web address **https://rpf.io/emoji** that links to a useful webpage. 

Add a new `<section>` for your link. Within the section, add a new paragraph that contains your link.

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 43
line_highlights: 46-48
---
     <p class="narrow hugefont spinme">🏆</p>         
  </section>

  <section>
     <p class="xcenter"><a href="https://rpf.io/emoji" target="_blank">More emoji!</a></p>
  </section>

--- /code ---

--- /task ---

--- task ---

**Test:** Look at your webpage and check that the link is centred on the page, underlined, and in a bold font. Click the link to open the emoji webpage in a new tab. 

The appearance of the link is set by a rule for `<a>` elements in your style file. 

--- /task ---

The `<blockquote>` tag is used when you want to quote someone. To give them credit, you can use the `<cite>` tag.

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
"Oceans of emotion can be transmitted through a text message, an emoji sequence, and a winking semicolon, but humans are hardwired to respond to visuals." - Jenna Wortham.
</p>

--- task ---

Add another section for your quote.  

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 46
line_highlights: 50-55
---
  <section>
     <p class="xcenter"><a href="https://rpf.io/emoji" target="_blank">More emoji!</a></p>
  </section>

  <section class="wrap">
       <blockquote>
           <p>"Oceans of emotion can be transmitted through an emoji sequence"</p>
           <cite>- Jenna Wortham.</cite>
       </blockquote>
  </section>

--- /code ---

--- /task ---


--- task ---

**Test:** Look at your webpage and see that the quote is styled in a large font and the citation is in a small font below. 

This is because your style file contains rules for styling `<blockquote>` and `<cite>` elements. 

<div>
<iframe src="https://trinket.io/embed/html/4603f442a9?outputOnly=true" width="500" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>
</div>

--- /task ---



