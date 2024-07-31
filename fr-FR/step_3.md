## Animer un emoji

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Au cours de cette étape, tu ajouteras un grand emoji animé pour rendre ta page web plus attrayante pour les gens qui la consulte.
</div>
<div>
<iframe src="https://editor.raspberrypi.org/fr-FR/embed/viewer/top-5-emoji-list-step-3" width="500" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>
</div>

--- task ---

Tu utiliseras un grand emoji trophée pour souligner qu’il s’agit des emojis les plus populaires.

Ajoute un nouveau paragraphe `<p>` à ton `<section>` pour afficher l'emoji trophée 🏆.

La classe `hugefont` rend le texte de l'emoji très grand.

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
          <li>🤣 – Se rouler par terre en riant.</li>
          <li>👍👍🏻👍🏼👍🏽👍🏾👍🏿 – Pouce vers le haut.</li>
          <li>😭 – Visage qui pleure à chaudes larmes.</li>
          <li>🙏🙏🏻🙏🏽🙏🏽🙏🏾🙏🏿 – Mains jointes.</li>
          <li>😘 – Visage envoyant un baiser.</li>
        </ol>
        <p class="hugefont">🏆</p>  
      </section>

--- /code ---

--- /task ---

--- task ---

**Test :** clique sur le bouton **Run**.

Vérifie que l'emoji du grand trophée apparaît sous la liste.

--- /task ---

--- task ---

Ajoute la classe `wrap` à ton `<section>` pour rendre ton site web responsive en ajustant la mise en page en fonction de l'espace disponible.

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
           <li>🤣 – Se rouler par terre en riant.</li>
           <li>👍👍🏻👍🏼👍🏽👍🏾👍🏿 – Pouce vers le haut.</li>
           <li>😭 – Visage qui pleure à chaudes larmes.</li>
           <li>🙏🙏🏻🙏🏽🙏🏽🙏🏾🙏🏿 – Mains jointes.</li>
           <li>😘 – Visage envoyant un baiser.</li>
         </ol>
         <p class="hugefont">🏆</p>        
      </section>

--- /code ---

--- /task ---

--- task ---

**Test :** clique sur le bouton **Run**.

Vérifie que le trophée apparaît ensuite dans la liste, si la page web est suffisamment large. La liste et le trophée doivent avoir la même largeur.

--- /task ---

La feuille de style comprend également des classes `wide` et `narrow` que tu peux utiliser pour modifier la largeur de différents éléments :

- Ajoute la classe `wide` à la balise `<ol>`

- Ajoute la classe `narrow` à ton paragraphe d'emoji trophée

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
           <li>🤣 – Se rouler par terre en riant.</li>
           <li>👍👍🏻👍🏼👍🏽👍🏾👍🏿 – Pouce vers le haut.</li>
           <li>😭 – Visage qui pleure à chaudes larmes.</li>
           <li>🙏🙏🏻🙏🏽🙏🏽🙏🏾🙏🏿 – Mains jointes.</li>
           <li>😘 – Visage envoyant un baiser.</li>
         </ol>
       <p class="hugefont narrow">🏆</p>     
     </section>
 
--- /code ---

--- /task ---

--- task ---

**Test :** clique sur le bouton **Run**.

Vérifie que la liste est plus large. Si ta page web est suffisamment large, le trophée apparaît à droite.

--- /task ---

Tu peux également utiliser HTML et CSS pour créer des **animations** qui changent des éléments sur une page web.

Une règle CSS `@keyframes` peut être modifiée au fil du temps. Tu peux modifier la couleur, la position, la taille et la rotation d'un élément, ainsi que de nombreuses autres propriétés.

`@keyframes` contrôle l'apparence de l'élément lorsqu'un pourcentage de l'animation en cours est terminé.

--- task ---

**Rechercher :** recherche la classe `.spinme` en haut du fichier `animation.css`. La classe `.spinme` a été créée pour toi et exécute une animation CSS appelée `rotate-center` qui tourne à partir d'une position de départ de 0 degrés et se termine à 360 degrés.

La ligne `animation: rotate-center linear 8s 2;` indique à la classe d'utiliser l'animation `rotate-center` avec un timing `linear` (linéaire) afin qu'elle s'exécute à la même vitesse tout au long. L'animation dure huit secondes et se répète deux fois.

--- code ---
---
language: CSS
filename: animation.css
line_numbers: true
line_number_start: 1
line_highlights: 1-4
---
.spinme {
  animation: rotate-center linear 8s 2; /* Temps nécessaire à l'animation et nombre de répétitions */
  display: inline-block;
}

@keyframes rotate-center {
  /* Le code d'animation de rotation */
  0% { 
    /* Rotation de 0 à 360 degrés */
    transform: rotate(0);
  }
  100% {
    transform: rotate(360deg);
  }
}
 
--- /code ---

--- /task ---

--- task ---

Retourne au fichier `index.html`.

Ajoute la classe `spinme` au paragraphe contenant le trophée.

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
                <li>🤣 – Se rouler par terre en riant.</li>
                <li>👍👍🏻👍🏼👍🏽👍🏾👍🏿 – Pouce vers le haut.</li>
                <li>😭 – Visage qui pleure à chaudes larmes.</li>
                <li>🙏🙏🏻🙏🏽🙏🏽🙏🏾🙏🏿 – Mains jointes.</li>
                <li>😘 – Visage envoyant un baiser.</li>
            </ol>
            <p class="hugefont narrow spinme">🏆</p>         
        </section>

--- /code ---

--- /task ---

--- task ---

**Test :** clique sur le bouton **Run**.

Ton trophée devrait tourner deux fois chaque fois que tu charges la page (en cliquant sur le bouton **Run**).

--- /task ---

--- task ---

Retourne au fichier `animation.css`.

**Choisir :** modifie les deux dernières valeurs de la ligne `animation: rotate-center linear 8s 2;` pour personnaliser ton animation.

- Que se passe-t-il si tu exécutes l'animation pendant plus de huit secondes ?
- Veux-tu que ton animation soit exécutée plus de deux fois ?

<iframe src="https://editor.raspberrypi.org/fr-FR/embed/viewer/top-5-emoji-list-step-3" width="600" height="700" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>

--- /task ---
