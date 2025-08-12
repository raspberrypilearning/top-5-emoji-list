\--- question ---

---

## legend: Vraag 3 van 3

Deze HTML- en CSS-code zou transparantie op de sectie moeten toepassen, maar het werkt niet. Welke regel moet je wijzigen?

## --- code ---

language: css
filename: style.css
line_numbers: true
-------------------------------------------------------

.transparent {
opacity: 1.00;
}

\--- /code ---

## --- code ---

language: html
filename: index.html
line_numbers: true
-------------------------------------------------------

<main class="transparent">
      <section>    
        <p>Dit is de inleiding.</p>
      </section>
</main>

\--- /code ---

\--- choices ---

- ( ) Regel 1 in `style.css`

  \--- feedback ---

  Probeer het nog eens. Deze regel is juist. Wanneer je een regel schrijft, heb je een punt `.` nodig vóór de naam van de class.

  \--- /feedback ---

- (x) Regel 2 in `style.css`

  \--- feedback ---

  Juist. Een dekking van `1.0` betekent helemaal niet transparant! Je zou dit kunnen veranderen naar een getal lager dan 0.75, om het probleem op te lossen.

  \--- /feedback ---

- ( ) Regel 1 in `index.html`

  \--- feedback ---

Niet helemaal. Dit is de juiste manier om een CSS-class aan een HTML-element toe te voegen.

\--- /feedback ---

- ( ) Regel 2 in `index.html`

  \--- feedback ---

Niet helemaal. De sectie bevindt zich binnen het `<main>` element, dus als de dekking correct is ingesteld voor `<main>`, is de sectie ook transparant.

\--- /feedback ---

\--- /choices ---

\--- /question ---
