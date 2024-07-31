## Ajouter une image d'arrière-plan

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">

Ajoute un arrière-plan emoji coloré et rends la partie principale de la page transparente afin que tu puisses voir l'image à travers le contenu principal.

</div>
<div>
<iframe src="https://editor.raspberrypi.org/fr-FR/embed/viewer/top-5-emoji-list-step-4" width="500" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>
</div>

La propriété CSS `background-image` te permet de définir une image comme arrière-plan de ta page web.

--- task ---

**Rechercher :** dans `style.css`, recherche la règle CSS `body` et **décommente** la ligne `background-image` pour définir l'image d'arrière-plan de ta page web.

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 44
line_highlights: 47
---
/* ajoute une image d'arrière-plan au corps */

body {
  background-image: url('emojis.png'); /* Décommenter et changer le nom du fichier pour ajouter une image d'arrière-plan
  /*background-repeat: repeat;*/ /* Fait répéter l'image */
  /*background-size: cover;*/ /* Fait en sorte que l'image couvre l'ensemble du conteneur */
}

--- /code ---

--- /task ---

--- task ---

**Test :** clique sur le bouton **Run**.

Tu devrais voir l’image emoji colorée sur les bords de ta page web.

**Astuce** tu peux avoir besoin de voir ta zone de sortie pour voir l'image d'arrière-plan.

**Astuce :** si tu visualises ta page web sur un téléphone mobile, fais pivoter l'écran en mode paysage.

--- /task ---

**Opacité** signifie à quel point il est difficile de voir à travers un objet. Une opacité de 1 signifie qu'un élément HTML est entièrement solide et que tu ne peux pas voir à travers. Une opacité de 0 signifie qu'un élément est complètement transparent.

--- task ---

**Rechercher :** dans le fichier `style.css`, recherche le commentaire `/* Ajouter un effet de transparence */`.

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 93
line_highlights: 93
---

/* Ajouter un effet de transparence */
 

--- /code ---

--- /task ---

Jusqu'à présent, tu as utilisé des classes CSS qui ont été créées pour toi. Maintenant, tu vas créer une nouvelle classe CSS appelée `transparent`, que tu peux utiliser pour rendre l'élément HTML `<main>` transparent.

Une opacité de '0.95' est légèrement transparente.

Ajoute la règle `.transparent` sous le commentaire.

--- task ---

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 93
line_highlights: 95-97
---

/* Ajouter un effet de transparence */
 
.transparent {
 opacity: 0.95;
}

--- /code ---

--- /task ---

Tu as ajouté une nouvelle classe CSS, mais maintenant tu dois l'utiliser.

--- task ---

Ajoute ta nouvelle classe `transparent` à `<main>` dans ton fichier HTML.

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

**Test :** clique sur le bouton **Run**.

Vérifie que la partie principale de ta page est légèrement transparente.

Que se passe-t-il si tu modifies `l'opacité` en `0.50`, `0.75` ou `0.90` ? Essaie différentes valeurs dans ta règle CSS et vois lequel tu préfères.

<div>
<iframe src="https://editor.raspberrypi.org/fr-FR/embed/viewer/top-5-emoji-list-step-4" width="500" height="700" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>

--- /task ---
