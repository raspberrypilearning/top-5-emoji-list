--- question ---

---
legend: Question 3 sur 3
---

Ce code HTML et CSS est censé appliquer la transparence à la section mais il ne fonctionne pas. Quelle ligne dois-tu changer ?

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
        <p>Ceci est l'introduction.</p>
      </section>
</main>

--- /code ---

--- choices ---

- ( ) Ligne 1 dans `style.css`

  --- feedback ---

  Réessaie. Cette ligne est correcte. Tu as besoin d'un point `.` avant le nom de la classe lors de l'écriture d'une règle.

  --- /feedback ---

- (x) Ligne 2 dans `style.css`

  --- feedback ---

  Correct. Une opacité de `1.0` signifie pas du tout transparent ! Tu peux remplacer ce chiffre par un nombre inférieur à un, tel que 0.75, pour résoudre le problème.

  --- /feedback ---

- ( ) Ligne 1 dans `index.html`

  --- feedback ---

Pas tout à fait. C'est la bonne façon d'ajouter une classe CSS à un élément HTML.

  --- /feedback ---

- ( ) Ligne 2 dans `index.html`

  --- feedback ---

Pas tout à fait. La section est à l'intérieur de l'élément `<main>`, donc si l'opacité est correctement définie pour `<main>`, la section est également transparente.

  --- /feedback ---

--- /choices ---

--- /question ---
