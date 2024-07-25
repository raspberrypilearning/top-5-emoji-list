## Animer plus d’emojis

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">

Dans cette étape, tu ajouteras des emojis animés à l’en-tête de ton site web.

</div>
<div>
<iframe src="https://editor.raspberrypi.org/en/embed/viewer/top-5-emoji-list-step-6" width="500" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>
</div>

Tu as rendu l’en-tête de ton site web attrayant en utilisant des couleurs vives et une police élégante. Les animations d'en-tête rendent le site web vraiment accrocheur pour tes visiteurs.

\--- task ---

Ajoute cinq emojis à ton en-tête. Utilise la classe `bigfont` pour les agrandir.

La balise `<span>` te permet d'ajouter ultérieurement différentes animations à chaque emoji.

## --- code ---

language: html
filename: index.html
line_numbers: true
line_number_start: 30
line_highlights: 32-36
-----------------------------------------------------------

  <header class="secondary border-bottom">
      <h1>Top 5 Emojis!</h1>
      
      <span class="bigfont">🤣</span>
      <span class="bigfont">😇</span>
      <span class="bigfont">😭</span>
      <span class="bigfont">🤩</span>
      <span class="bigfont">😘</span>
  </header>

\--- /code ---

\--- /task ---

\--- task ---

Clique sur le fichier `animation.css` et recherche la classe `bounceme`.

L'animation `bounce` s'exécute avec un timing 'ease', de sorte que l'animation commence et se termine lentement mais s'accélère au milieu.

## --- code ---

language: css
filename: animation.css
line_numbers: true
line_number_start: 17
line_highlights: 17-20
-----------------------------------------------------------

.bounceme {
animation: bounce ease 2s 3; /\* runs the 'bounce' animation with ease timing (slow start and end) for two seconds. Runs the animation twice. \*/
display: inline-block;
}

@keyframes bounce {
/\* The bounce animation code _/
0% {
transform: scale(1, 1) translateY(0); /_ Starting position and actual size _/
}
10% {
transform: scale(1.1, 0.9) translateY(0); /_ Grow width and shrink height for pre-bounce squash effect _/
}
30% {
transform: scale(1, 1) translateY(-6rem); /_ Return to actual size and move emoji up 100px from current position _/
}
50% {
transform: scale(1, 1) translateY(0); /_ Move emoji back to starting position \*/
}
}

\--- /code ---

**Regarder :** pour créer un effet de rebond, la propriété `scale` ajuste la taille et la propriété `translateY` déplace l'élément de haut en bas sur l'axe y.

\--- /task ---

\--- task ---

Clique sur le fichier `index.html` et ajoute la classe `bounceme` à l'emoji étoilé 🤩.

## --- code ---

language: html
filename: index.html
line_numbers: true
line_number_start: 30
line_highlights: 35
--------------------------------------------------------

  <header class="secondary border-bottom">
    <h1>Top 5 Emojis!</h1>
    
    <span class="bigfont">🤣</span>
    <span class="bigfont">😇</span>
    <span class="bigfont">😭</span>
    <span class="bigfont bounceme">🤩</span>
    <span class="bigfont">😘</span>
  </header>

\--- /code ---

\--- /task ---

\--- task ---

**Test :** clique sur le bouton **Run**.

Chaque fois que tu charges ta page, ton emoji frappé par une étoile 🤩 devrait rebondir trois fois.

**Débogage :**

\--- collapse ---

---

## title: Un emoji dans la liste rebondit au lieu d'un emoji dans l'en-tête !

Tu dois ajouter `bounceme` à un emoji dans le `<header>`, pas à l'emoji dans le `<ol>`.

\--- /collapse ---

\--- /task ---

Lorsque tu consultes une page web, la partie qui t'est visible s'appelle **viewport**. Un téléphone mobile a une fenêtre d'affichage beaucoup plus petite qu'un écran d'ordinateur de bureau.

Ton projet a déjà du code pour contrôler la taille et l'échelle de **viewport** à adapter à la largeur de l'appareil. Tu peux utiliser le viewport dans les animations pour faire le changement d'animation pour s'adapter à la fenêtre d'affichage.

\--- task ---

Clique sur le fichier `animation.css` et recherche la classe `rollmeleft`. Cela crée une animation de roulement à partir de la gauche.

Une combinaison de 'translate' et 'rotate' est utilisée pour créer le roulement.

## --- code ---

language: css
filename: animation.css
line_numbers: true
line_number_start: 62
line_highlights: 62-65
-----------------------------------------------------------

.rollmeleft {
animation: rollleft ease 8s 1;
display: inline-block;
}

@keyframes rollleft {
/\* The roll animation code \*/
from {
transform: translate(-60vw) rotate(0deg);
}

to {
transform: translate(0vw) rotate(360deg);
}
}

\--- /code ---

**Regarder :** ce code `translate` utilise `vw` (viewport-width). Le point de départ de '-60vw' est à 60 % à gauche de la position codée dans la fenêtre. L'animation se termine à la position codée '0vw'.

\--- /task ---

\--- task ---

Clique sur le fichier `index.html` et ajoute la classe `rollmeleft` à l'emoji qui se roule par terre en riant 🤣.

## --- code ---

language: html
filename: index.html
line_numbers: true
line_number_start: 30
line_highlights: 32
--------------------------------------------------------

  <header class="secondary border-bottom">
    <h1>Top 5 Emojis!</h1>
    
    <span class="bigfont rollmeleft">🤣</span>
    <span class="bigfont">😇</span>
    <span class="bigfont">😭</span>
    <span class="bigfont bounceme">🤩</span>
    <span class="bigfont">😘</span>
  </header>

\--- /code ---

\--- /task ---

\--- task ---

**Test :** clique sur le bouton **Run**.

Ton emoji qui roule par terre en riant 🤣 devrait se déplacer vers l'intérieur à partir de la gauche et pivoter au fur et à mesure.

**Astuce :** clique sur Run pour regarder à nouveau les animations.

\--- /task ---

\--- task ---

**Choisir :** ajoute des classes d'animation aux emojis restants 😇😭😘 pour terminer ton en-tête amusant et accrocheur.

Tu peux utiliser n'importe quelle animation du fichier `animation.css` :

- `spinme`
- `bounceme`
- `scaleme`
- `movemeleft`
- `movemeright`
- `rollmeleft`
- `rollmeright`

<div>
<iframe src="https://editor.raspberrypi.org/en/embed/viewer/top-5-emoji-list-step-6" width="500" height="500" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>

\--- /task ---
