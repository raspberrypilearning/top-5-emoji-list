
--- question ---

---
legend: Question 2 of 3
---

CSS styles can be applied to HTML code to decide on how the content should appear in the web browser. 

Below is some CSS code for styling a subheading. Which line of code would you change to make the subheading display on the right hand side.

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 1
line_highlights: 
---  

h2 {
  font: var(--title-font); 
  text-align: left; 
  padding: 1.5rem; 
}

--- /code ---

--- choices ---

- ( ) 1

  --- feedback ---

Take another look. The first line says that the **selector** which the rule applies to is the `h2` tag.
 
  --- /feedback ---

- ( ) 2

  --- feedback ---

Not quite. The second line says that the font for elements with the `h2` tag is provided by the `--title-font` **variable**.

  --- /feedback ---

- (x) 3

  --- feedback ---

  Correct! The third line allows you to change the alignment of the text. By changing `left` to `right`, the text would align on the right hand side. 

  --- /feedback ---

- ( ) 4

  --- feedback ---

  Try again. The fourth line allows you to adjust the space around the subheading. 

  --- /feedback ---

--- /choices ---

--- /question ---