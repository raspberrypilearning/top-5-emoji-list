## Voeg animatie toe aan meer emoji's

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">

In deze stap voeg je geanimeerde emoji's toe aan je website-kop.

</div>
<div>
<iframe src="https://editor.raspberrypi.org/nl-NL/embed/viewer/top-5-emoji-list-step-6" width="500" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>
</div>

Je hebt je website koptekst interessant gemaakt door vette kleuren en een stijlvol lettertype te gebruiken. Kopanimaties maken de website echt opvallend voor je kijkers.

--- task ---

Voeg vijf emoji's toe aan je header. Gebruik de `bigfont` class om ze groot te maken.

Met de `<span>` tag kun je later verschillende animaties aan elke emoji toevoegen.

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 30
line_highlights: 32-36
---

  <header class="secondary border-bottom">
      <h1>Top 5 Emoji's!</h1>
      <span class="bigfont">🤣</span>
      <span class="bigfont">😇</span>
      <span class="bigfont">😭</span>
      <span class="bigfont">🤩</span>
      <span class="bigfont">😘</span>
  </header>

--- /code ---

--- /task ---

--- task ---

Klik op het `animation.css` bestand en zoek de `bounceme` klas.

De `bounce` animatie werkt met `ease` timing zodat de animatie langzaam begint en eindigt maar in het midden versnellt.

--- code ---
---
language: css
filename: animation.css
line_numbers: true
line_number_start: 17
line_highlights: 17-20
---

.bounceme {
    animation: bounce ease 2s 3; /* voert de 'bounce' animatie met 'ease timing' (langzame start en einde) gedurende twee seconden. Voert de animatie 3 keer uit. */
    display: inline-block;
}

@keyframes bounce {
    /* De bounce-animatiecode */
    0% {
        transform: scale(1, 1) translateY(0); /* Beginpositie en werkelijke grootte */
    }
    10% {
        transform: scale(1.1, 0.9) translateY(0); /* Breedte vergroten en hoogte verkleinen voor pre bounce squash effect */
    }
    30% {
        transform: scale(1, 1) translateY(-6rem); /* Keer terug naar werkelijke grootte en verplaats emoji omhoog met 100px van de huidige positie */
    }
    50% {
        transform: scale(1, 1) translateY(0); /* Verplaats emoji terug naar startpositie */
    }
}

--- /code ---

**Kijk:** Om een bounce effect te maken, past de eigenschap `scale` de grootte aan en beweegt de eigenschap `translateY` het element omhoog en omlaag langs de y-as.

--- /task ---

--- task ---

Klik op het `index.html` bestand en voeg de `bounceme` class toe aan de star-struck emoji 🤩.

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 30
line_highlights: 35
---

  <header class="secondary border-bottom">
    <h1>Top 5 emoji's!</h1>
    <span class="bigfont">🤣</span>
    <span class="bigfont">😇</span>
    <span class="bigfont">😭</span>
    <span class="bigfont bounceme">🤩</span>
    <span class="bigfont">😘</span>
  </header>

--- /code ---

--- /task ---

--- task ---

**Test:** Klik op de **Run** knop.

Elke keer dat je je pagina laadt, zou je star-struck emoji 🤩 drie keer moeten stuiteren.

**Fouten oplossen:**

--- collapse ---

---
title: Een emoji in de lijst stuitert in plaats van een emoji in de kop!
---

Je moet `bounceme` toevoegen aan een emoji in de `<header>`, niet de emoji in de `<ol>`.

--- /collapse ---

--- /task ---

Als je op een webpagina kijkt, wordt het onderdeel dat voor jou zichtbaar is de **viewport** genoemd. Een mobiele telefoon heeft een veel kleinere viewport dan een desktop computerscherm.

Je project heeft al code om de **viewport** grootte en schaal te beheren en aan te passen aan de apparaatbreedte. Je kunt viewport in animaties gebruiken om de animatie te veranderen om aan de viewport te voldoen.

--- task ---

Klik op het `animation.css` bestand en zoek de `rollmeleft` class. Hierdoor ontstaat een rollende animatie van links.

Een combinatie van `translate` en `rotate` wordt gebruikt om de rol te maken.

--- code ---
---
language: css
filename: animation.css
line_numbers: true
line_number_start: 62
line_highlights: 62-65
---

.rollmeleft {
  animation: rollleft ease 8s 1;
  display: inline-block;
}

@keyframes rollleft {
  /* De rolanimatiecode */
  from {
    transform: translate(-60vw) rotate(0deg);
  }

  to {
    transform: translate(0vw) rotate(360deg);
  }
}

--- /code ---

**Kijk:** Deze `translate` code gebruikt `vw` (viewport-width, viewport-breedte). Het startpunt van `-60vw` is 60% links van de gecodeerde positie op de viewport. De animatie eindigt op de gecodeerde positie `0vw`.

--- /task ---

--- task ---

Klik op het `index.html` bestand en voeg de `rollmeleft` class toe aan de rollen over de vloer van het lachen emoji 🤣.

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 30
line_highlights: 32
---

  <header class="secondary border-bottom">
    <h1>Top 5 emoji's!</h1>
    <span class="bigfont rollmeleft">🤣</span>
    <span class="bigfont">😇</span>
    <span class="bigfont">😭</span>
    <span class="bigfont bounceme">🤩</span>
    <span class="bigfont">😘</span>
  </header>

--- /code ---

--- /task ---

--- task ---

**Test:** Klik op de **Run** knop.

Je rollende over de vloer van het lachen emoji 🤣 moet van links naar binnen komen en draaien terwijl hij beweegt.

**Tip:** Klik op Run om de animaties opnieuw te bekijken.

--- /task ---

--- task ---

**Kies:** Voeg animation classes toe aan de resterende emoji's 😇😭😘 om je leuke opvallende kop af te maken.

Je kunt elke animatie gebruiken uit het `animation.css` bestand:

- `spinme`
- `bounceme`
- `scaleme`
- `movemeleft`
- `movemeright`
- `rollmeleft`
- `rollmeright`

<div>
<iframe src="https://editor.raspberrypi.org/nl-NL/embed/viewer/top-5-emoji-list-step-6" width="500" height="500" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>

--- /task ---
