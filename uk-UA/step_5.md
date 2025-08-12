## Додай цитату та посилання

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">

У цьому кроці ти використовуватимеш такі три теги HTML: `<blockquote>` та `<cite>` для додавання цитат і `<a>` для додавання посилань на інші вебсторінки.

</div>
<div>
<iframe src="https://editor.raspberrypi.org/en/embed/viewer/top-5-emoji-list-step-5" width="500" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>
</div>

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
<span style="color: #0faeb0">Гіперпосилання</span> (або гіперлінк) — посилання на іншу вебсторінку, на яке можна клікнути. Посилання зазвичай підкреслені або якось додатково виділені, щоб відокремити їх від решти тексту. 
</p>

У мові HTML для створення посилань використовують тег `<a>`:

- Текст посилання, який видно на сторінці, розміщується між `<a>` і `</a>`
- Атрибут `href` містить вебадресу (що зазвичай починається з «https://») сторінки, на яку має вести посилання
- Ти також можеш додати `target="_blank"`, щоби сторінка посилання відкривалася в новій вкладці веббраузера, а не замінювала собою сторінку, на якій ти знаходишся.

\--- task ---

Ми створили коротку вебадресу **https://rpf.io/emoji**, яка веде на корисну вебсторінку.

Додай нову секцію `<section>`, що використовує клас `xcentre` та містить твоє посилання.

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

**Протестуй:** натисни на кнопку **Run**.

Переглянь свою вебсторінку та переконайся, що посилання розташоване по центру, підкреслене та виділене жирним шрифтом.

Натисни на посилання, щоб відкрити сторінку з емоджі у новій вкладці.

Зовнішній вигляд посилання визначається правилом для елементів `<a>` у твоєму файлі зі стилями.

\--- /task ---

Тег `<blockquote>` використовується, щоб процитувати когось.

Щоб вказати імʼя людини, якій належить цитата, використовуй тег `<cite>`.

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
«Океани емоцій можна передати через текстове повідомлення, пару емоджі та жартівливу крапку з комою, адже люди запрограмовані реагувати на візуальну інформацію». - Дженна Вортем.
</p>

\--- task ---

Додай ще одну секцію для цитати.

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

**Протестуй:** натисни на кнопку **Run**.

Подивися на свою сторінку. Цитата має бути оформлена великим шрифтом, а імʼя авторки — меншим шрифтом унизу.

Це тому, що твій файл зі стилями містить правила для стилізації елементів `<blockquote>` та `<cite>`.

<div>
<iframe src="https://editor.raspberrypi.org/en/embed/viewer/top-5-emoji-list-step-5" width="600" height="1000" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>

\--- /task ---



