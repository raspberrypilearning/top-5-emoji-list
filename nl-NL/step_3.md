## Voeg animatie toe aan een emoji

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
In deze stap voeg je een grote geanimeerde emoji toe om je webpagina interessanter te maken voor kijkers.
</div>
<div>
<iframe src="https://editor.raspberrypi.org/nl-NL/embed/viewer/top-5-emoji-list-step-3" width="500" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>
</div>

--- task ---

Je gebruikt een grote trofee-emoji om te benadrukken dat dit de populairste emoji's zijn.

Voeg een nieuw alinea `<p>` toe aan je `<section>` om de trofee emoji 🏆 te tonen.

De `hugefont` class maakt de emoji tekst heel groot.

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
          <li>🤣 – Rollend over de vloer van het lachen.</li>
          <li>👍👍🏻👍🏼👍🏽👍🏾👍🏿 – Goed zo.</li>
          <li>😭 – Gezicht dat hard huilt.</li>
          <li>🙏🙏🏻🙏🏽🙏🏽🙏🏾🙏🏿 – Gevouwen handen.</li>
          <li>😘 – Gezicht dat zoen geeft.</li>
        </ol>
        <p class="hugefont">🏆</p>  
      </section>

--- /code ---

--- /task ---

--- task ---

**Test:** Klik op de **Run** knop.

Controleer of de grote trofee emoji onder de lijst verschijnt.

--- /task ---

--- task ---

Voeg de `wrap` class toe aan jouw `<section>` om jouw website te laten reageren door de lay-out aan te passen aan de beschikbare ruimte.

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
           <li>🤣 – Rollend over de vloer van het lachen.</li>
           <li>👍👍🏻👍🏼👍🏽👍🏾👍🏿 – Goed zo.</li>
           <li>😭 – Gezicht dat hard huilt.</li>
           <li>🙏🙏🏻🙏🏽🙏🏽🙏🏾🙏🏿 – Gevouwen handen.</li>
           <li>😘 – Gezicht dat zoen geeft.</li>
         </ol>
         <p class="hugefont">🏆</p>        
      </section>

--- /code ---

--- /task ---

--- task ---

**Test:** Klik op de **Run** knop.

Controleer of de trofee als volgende in de lijst verschijnt, als de webpagina breed genoeg is. De lijst en de trofee zouden dezelfde breedte moeten hebben.

--- /task ---

Het style sheet bevat ook `wide` en `narrow` classes die je kunt gebruiken om de breedte van de verschillende elementen te wijzigen:

- Voeg de `wide` class toe aan de `<ol>` tag

- Voeg de `narrow` class toe aan je trofee emoji alinea

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
           <li>🤣 – Rollend over de vloer van het lachen.</li>
           <li>👍👍🏻👍🏼👍🏽👍🏾👍🏿 – Goed zo.</li>
           <li>😭 – Gezicht dat hard huilt.</li>
           <li>🙏🙏🏻🙏🏽🙏🏽🙏🏾🙏🏿 – Gevouwen handen.</li>
           <li>😘 – Gezicht dat zoen geeft.</li>
         </ol>
       <p class="hugefont narrow">🏆</p>     
     </section>
 
--- /code ---

--- /task ---

--- task ---

**Test:** Klik op de **Run** knop.

Controleer of de lijst breder is. Als je webpagina breed genoeg is, verschijnt de trofee aan de rechterkant.

--- /task ---

Je kunt ook HTML en CSS gebruiken om **animaties** te maken die elementen op een webpagina wijzigen.

Een CSS `@keyframes` regel kan worden ingesteld om na verloop van tijd te veranderen. Je kunt de kleur, positie, grootte en rotatie van een element wijzigen, en nog veel meer eigenschappen.

`@keyframes` bepalen hoe het element eruit moet zien wanneer een percentage van de lopende animatie is voltooid.

--- task ---

**Zoeken:** Zoek naar de `.spinme` class bovenaan het `animation.css` bestand. De `.spinme` class is voor jou gemaakt en het heeft een CSS animatie genaamd 'rotate-center' die draait vanaf een startpositie van 0 graden en bij 360 graden eindigt.

De regel `animation: rotate-center lineair 8s 2;` geeft de opdracht aan de class om de `rotate-center` animatie te gebruiken met `lineair` timing, zodat deze met steeds dezelfde snelheid doorloopt. De animatie duurt acht seconden en wordt twee keer herhaald.

--- code ---
---
language: CSS
filename: animation.css
line_numbers: true
line_number_start: 1
line_highlights: 1-4
---
.spinme {
  animation: rotate-center linear 8s 2; /* Tijd nodig voor animatie en aantal herhalingen */
  display: inline-block;
}

@keyframes rotate-center {
  /* De rotatie-animatiecode */
  0% { 
    /* Roteren van 0 tot 360 graden */
    transform: rotate(0);
  }
  100% {
    transform: rotate(360deg);
  }
}
 
--- /code ---

--- /task ---

--- task ---

Ga terug naar het `index.html` bestand.

Voeg de `spinme` class toe aan de alinea die de trofee bevat.

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
                <li>🤣 – Rollend over de vloer van het lachen.</li>
                <li>👍👍🏻👍🏼👍🏽👍🏾👍🏿 – Goed zo.</li>
                <li>😭 – Gezicht dat hard huilt.</li>
                <li>🙏🙏🏻🙏🏽🙏🏽🙏🏾🙏🏿 – Gevouwen handen.</li>
                <li>😘 – Gezicht dat zoen geeft.</li>
            </ol>
            <p class="hugefont narrow spinme">🏆</p>         
        </section>

--- /code ---

--- /task ---

--- task ---

**Test:** Klik op de **Run** knop.

Je trofee zou tweemaal draaien als je de pagina laadt (door op de **Run** knop te klikken).

--- /task ---

--- task ---

Ga terug naar het `animation.css` bestand.

**Kies:** Verander de laatste twee waarden in de regel `animation: rotate-center linear 8s 2;` om je animatie aan te passen.

- Wat gebeurt er als je de animatie langer dan acht seconden uitvoert?
- Wil je dat je animatie meer dan twee keer wordt uitgevoerd?

<iframe src="https://editor.raspberrypi.org/nl-NL/embed/viewer/top-5-emoji-list-step-3" width="600" height="700" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>

--- /task ---
