## Add quote and link

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">

In this step you will use three more HTML tags: `<blockquote>` and `<cite>` for including quotations and `<a>` for adding links to other web pages. 

</div>
<div>
<iframe src="https://trinket.io/embed/html/4603f442a9?outputOnly=true" width="390" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>
</div>
</div>

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
A <span style="color: #0faeb0">hyperlink</span> is a clickable link to another web page. Links are usually underlined or otherwise styled to make them standout. 
</p>

In HTML the `<a>` tag is used to create links. 

+ You put the link text that will appear on the web page inside `<a>` and `</a>` 
+ The `href` attribute provides the web address (usually beginning with 'https:') of the page you want to link to. 
+ You can also add `target="_blank"` to make the linked web page open in a new tab in the web browser instead of replacing the current web page.  

--- task ---

We have created a short web address 'https://rpf.io/emoji' that links to a useful web page. 

Add a new `<section>` for your link. Within the section, add a new paragraph that contains your link:

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 47
line_highlights: 50-52
---
     <p class="narrow hugefont spinme">🏆</p>         
  </section>

  <section>
     <p class="xcenter"><a href="https://rpf.io/emoji" target="_blank">More emoji!</a></p>
  </section>

--- /code ---

--- /task ---

--- task ---

**Test:** Look at your web page and see the link centered on the page, underlined and in a bold font. Click the link to open the emoji web page in a new tab. 

The appearance of the link is set by a rule for `<a>` elements in your style file. 

--- /task ---

The `<blockquote>` tag is used when you want to quote someone. To give them credit you can use the `<cite>` tag.

<blockquote style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
           <p>"Oceans of emotion can be transmitted through a text message, an emoji sequence, and a winking semicolon, but humans are hardwired to respond to visuals."</p>
           <cite>- Jenna Wortham.</cite>
</blockquote>

--- task ---

Add another section for your quote.  

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 47
line_highlights: 51-56
---
  <section>
     <p class="xcenter"><a href="https://rpf.io/emoji" target="_blank">More emoji!</a></p>
  </section>

  <section>
       <blockquote>
           <p>"Oceans of emotion can be transmitted through an emoji sequence"</p>
           <cite>- Jenna Wortham.</cite>
       </blockquote>
  </section>

--- /code ---

--- /task ---


--- task ---

**Test:** Look at your web page and see that the quote is styled in a large font and the citation is in a small font below. 

This is because your style file contains rules for styling `<blockquote>` and `<cite>` elements. 

<div>
<iframe src="https://trinket.io/embed/html/4603f442a9?outputOnly=true" width="390" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>
</div>

--- /task ---



