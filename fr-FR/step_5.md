## Ajouter une citation et un lien

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">

Dans cette étape, tu utiliseras trois balises HTML supplémentaires : `<blockquote>` et `<cite>` pour inclure des citations et `<a>` pour ajouter des liens vers d'autres pages web.

</div>
<div>
<iframe src="https://editor.raspberrypi.org/fr-FR/embed/viewer/top-5-emoji-list-step-5" width="500" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>
</div>

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
Un <span style="color: #0faeb0">lien hypertexte</span> est un lien cliquable vers une autre page web. Les liens sont généralement soulignés ou stylisés pour les séparer du reste du texte. 
</p>

En HTML, la balise `<a>` est utilisée pour créer des liens :

- Tu places le texte du lien qui apparaît sur la page web entre `<a>` et `</a>`
- L'attribut `href` fournit l'adresse web (commençant généralement par 'https://') de la page vers laquelle tu souhaites créer un lien
- Tu peux également ajouter `target="_blank"` pour ouvrir la page web liée dans un nouvel onglet du navigateur web, au lieu que la nouvelle page remplace la page web actuelle.

--- task ---

Nous avons créé une courte adresse web **https://rpf.io/emoji** qui renvoie à une page web utile.

Ajoute un nouveau `<section>` qui utilise la classe `xcentre` et inclut ton lien.

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 43
line_highlights: 46-48
---
            <p class="narrow hugefont spinme">🏆</p>         
        </section>

        <section class="xcenter">
            <a href="https://rpf.io/emoji" target="_blank">Plus d'emojis !</a>
        </section>

--- /code ---

--- /task ---

--- task ---

**Test :** clique sur le bouton **Run**.

Regarde ta page web et vérifie que le lien est centré sur la page, souligné et en gras.

Clique sur le lien pour ouvrir la page web des emojis dans un nouvel onglet.

L'apparence du lien est définie par une règle pour les éléments `<a>` dans ton fichier de style.

--- /task ---

La balise `<blockquote>` est utilisée lorsque tu veux citer quelqu'un.

Pour leur donner du crédit, tu peux utiliser la balise `<cite>`.

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
« Des océans d'émotions peuvent être transmis via un message texte, une séquence d'émoticônes et un point-virgule clignotant, mais les humains sont programmés pour réagir aux visuels. » - Jenna Wortham.
</p>

--- task ---

Ajoute une autre section pour ta citation.

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 46
line_highlights: 50-55
---
        <section class="xcenter">
            <a href="https://rpf.io/emoji" target="_blank">Plus d'emojis !</a>
        </section>

        <section class="wrap">
            <blockquote>
                <p>« Des océans d'émotions peuvent être transmis par une séquence d'emoji »</p>
                <cite>- Jenna Wortham.</cite>
            </blockquote>
        </section>

--- /code ---

--- /task ---

--- task ---

**Test :** clique sur le bouton **Run**.

Regarde ta page web. La citation doit être rédigée en grande police et le crédit en petite police en dessous.

En effet, ton fichier de style contient des règles pour styliser les éléments `<blockquote>` et `<cite>`.

<div>
<iframe src="https://editor.raspberrypi.org/fr-FR/embed/viewer/top-5-emoji-list-step-5" width="600" height="1000" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>

--- /task ---
