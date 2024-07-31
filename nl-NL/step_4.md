## Voeg een achtergrondafbeelding toe

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">

Voeg een kleurrijke emoji achtergrond toe en maak het hoofddeel van de pagina transparant, zodat je de afbeelding door de hoofdinhoud kunt zien.

</div>
<div>
<iframe src="https://editor.raspberrypi.org/nl-NL/embed/viewer/top-5-emoji-list-step-4" width="500" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>
</div>

De CSS `background-image` eigenschap laat je toe om een afbeelding als achtergrond voor je webpagina in te stellen.

--- task ---

**Zoek:** In `style.css`, vind je de CSS `body` regel en **uncomment** (verwijder de opmerking-tekens) de `background-image` regel om de achtergrondafbeelding voor je webpagina in te stellen.

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 44
line_highlights: 47
---
/* voeg een achtergrondafbeelding toe aan de hoofdtekst */

body {
  background-image: url('emojis.png'); /* Verwijder commentaar en wijzig de bestandsnaam om een achtergrondafbeelding toe te voegen
  /*background-repeat: repeat;*/ /* Laat de afbeelding herhalen */
  /*background-size: cover;*/ /* Zorg ervoor dat de afbeelding de hele container bedekt */
}

--- /code ---

--- /task ---

--- task ---

**Test:** Klik op de **Run** knop.

Je zou de kleurrijke emoji-afbeelding aan de randen van je webpagina moeten zien.

**Tip** Je moet mogelijk je uitvoergebied bekijken om de achtergrondafbeelding te zien.

**Tip:** Als je jouw webpagina op een mobiele telefoon weergeeft, draai dan het scherm in liggende modus.

--- /task ---

**Ondoorzichtigheid** betekent hoe moeilijk het is om door een object heen te kijken. Een ondoorzichtigheid van 1 betekent dat een HTML-element volledig effen is en je er niet doorheen kunt kijken. Een ondoorzichtigheid van 0 betekent dat een element volledig transparant is.

--- task ---

**Zoek:** Zoek in het bestand `style.css` de opmerking `/* Een transparant effect toevoegen */`.

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 93
line_highlights: 93
---

/* Voeg een transparant effect toe */
 

--- /code ---

--- /task ---

Tot nu toe heb je CSS-classes gebruikt die voor jou vooraf zijn gemaakt. Nu ga je een nieuwe CSS-class maken met de naam `transparent`, die je kunt gebruiken om het `<main>` HTML-element transparant te maken.

Een dekking van `0.95` is enigszins transparant.

Voeg de `.transparent`-regel toe onder de opmerking.

--- task ---

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 93
line_highlights: 95-97
---

/* Voeg een transparant effect toe */
 
.transparent {
 opacity: 0.95;
}

--- /code ---

--- /task ---

Je hebt een nieuwe CSS-class toegevoegd, maar nu moet je deze ook gaan gebruiken.

--- task ---

Voeg je nieuwe `transparent` class toe aan `<main>` in je HTML-bestand.

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 34
line_highlights: 34
---

<main class="transparent">
  <section class="wrap">    
    <ol class="wide">

--- /code ---

--- /task ---

--- task ---

**Test:** Klik op de **Run** knop.

Controleer of het hoofddeel van jouw pagina enigszins transparant is.

Wat gebeurt er als je de ‘dekking’ wijzigt in ‘0.50’, ‘0.75’ of ‘0.90’? Probeer verschillende waarden in je CSS-regel en kijk welke je verkiest.

<div>
<iframe src="https://editor.raspberrypi.org/nl-NL/embed/viewer/top-5-emoji-list-step-4" width="500" height="700" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>

--- /task ---
