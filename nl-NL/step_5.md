## Voeg een quote en een link toe

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">

In deze stap gebruik je nog drie HTML-tags: `<blockquote> en `<cite>`om citaten en`<a>\` toe te voegen aan andere webpagina's.

</div>
<div>
<iframe src="https://editor.raspberrypi.org/en/embed/viewer/top-5-emoji-list-step-5" width="500" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>
</div>

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
Een <span style="color: #0faeb0">hyperlink</span> is een klikbare link naar een andere webpagina. Links zijn meestal onderstreept of op een andere manier opgemaakt om ze van de rest van de tekst te scheiden. 
</p>

In HTML wordt de tag `<a>` gebruikt om links te maken:

- Je plaatst de link tekst die verschijnt op de webpagina in `<a>` en `</a>`
- Het `href` attribuut biedt het webadres (begint meestal met 'https://') van de pagina waarnaar je wilt linken
- Je kunt ook `target="_blank"` toevoegen om de gekoppelde webpagina te openen in een nieuw tabblad in de webbrowser, in plaats van via de nieuwe pagina de huidige webpagina te vervangen.

\--- task ---

We hebben een kort webadres **https://rpf.io/emoji** gemaakt dat linkt naar een nuttige webpagina.

Voeg een nieuwe '<section>' toe die de 'xcentre' class gebruikt en je link bevat.

## --- code ---

language: html
filename: index.html
line_numbers: true
line_number_start: 43
line_highlights: 46-48
-----------------------------------------------------------

```
        <p class="narrow hugefont spinme">🏆</p>         
    </section>

    <section class="xcenter">
        <a href="https://rpf.io/emoji" target="_blank">More emojis!</a>
    </section>
```

\--- /code ---

\--- /task ---

\--- task ---

**Test:** Klik op de **Run** knop.

Bekijk je webpagina en controleer of de link gecentreerd is op de pagina, en in een vet lettertype.

Klik op de link om de emoji webpagina in een nieuw tabblad te openen.

Het uiterlijk van de link is ingesteld door een regel voor `<a>` elementen in je stijlbestand.

\--- /task ---

De `<blockquote>` tag wordt gebruikt wanneer je iemand wilt citeren.

Om ze een vermelding te geven, kun je de `<cite>` tag gebruiken.

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
"Oceanen van emoties kunnen worden overgedragen via een sms-bericht, een emoji-reeks en een knipogende puntkomma, maar mensen zijn geprogrammeerd om op beelden te reageren." - Jenna Wortham.
</p>

\--- task ---

Nog een sectie toevoegen voor je quote.

## --- code ---

language: html
filename: index.html
line_numbers: true
line_number_start: 46
line_highlights: 50-55
-----------------------------------------------------------

```
    <section class="xcenter">
        <a href="https://rpf.io/emoji" target="_blank">More emojis!</a>
    </section>

    <section class="wrap">
        <blockquote>
            <p>"Oceans of emotion can be transmitted through an emoji sequence"</p>
            <cite>- Jenna Wortham.</cite>
        </blockquote>
    </section>
```

\--- /code ---

\--- /task ---

\--- task ---

**Test:** Klik op de **Run** knop.

Kijk naar je webpagina. Het citaat moet in een groot lettertype worden opgemaakt en het citaat staat hieronder in een klein lettertype.

Dit is omdat je stijlbestand regels bevat voor styling `<blockquote>` en `<cite>` elementen.

<div>
<iframe src="https://editor.raspberrypi.org/en/embed/viewer/top-5-emoji-list-step-5" width="600" height="1000" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>

\--- /task ---



