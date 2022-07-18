
--- question ---

---
legend: Question 3 of 3
---

This HTML and CSS code is supposed to apply transparency to the section but it’s not working. Which line do you need to change? 

--- code ---
---
language: css
filename: style.css
line_numbers: true
---
.transparent {
  opacity: 1.00;
}

--- /code ---

--- code ---
---
language: html
filename: index.html
line_numbers: true
---
<main class="transparent">
      <section>    
        <p>This is the introduction.</p>
      </section>
</main>

--- /code ---

--- choices ---

- ( ) Line 1 in `style.css`

  --- feedback ---

  Try again. This line is correct. You need a dot '.' before the name of the class when writing a rule. 
 
  --- /feedback ---

- (x) Line 2 in `style.css`

  --- feedback ---

  Correct. An opacity of `1.0` means not at all transparent! You could change this to a number below one, such as '0.75', to fix the problem. 

  --- /feedback ---

- ( ) Line 1 in `index.html`

  --- feedback ---

 Not quite. This is the correct way to add a CSS class to an HTML element. 
 
  --- /feedback ---

- ( ) Line 2 in `index.html`

  --- feedback ---

 Not quite. The section is inside the `<main>` element so if opacity is correctly set for main, the section is also transparent. 

  --- /feedback ---


--- /choices ---

--- /question ---
