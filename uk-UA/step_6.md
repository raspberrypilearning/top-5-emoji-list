## Створи анімації для інших емоджі

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">

На цьому кроці ти додаси до заголовка свого вебсайту анімовані емоджі.

</div>
<div>
<iframe src="https://editor.raspberrypi.org/en/embed/viewer/top-5-emoji-list-step-6" width="500" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>
</div>

Заголовок твого вебсайту вже досить цікавий завдяки яскравим кольорам і стильним шрифтам. Анімація заголовку зробить сторінку справді захопливою для твоїх відвідувачів.

\--- task ---

Додай п'ять емоджі до заголовка. Використай клас `bigfont`, щоб зробити їх великими.

Тег `<span>` дасть тобі змогу додати до кожного емоджі різні анімації.

## --- code ---

language: html
filename: index.html
line_numbers: true
line_number_start: 30
line_highlights: 32-36
-----------------------------------------------------------

  <header class="secondary border-bottom">
      <h1>Пʼять найкращих емоджі!</h1>
      
      <span class="bigfont">🤣</span>
      <span class="bigfont">😇</span>
      <span class="bigfont">😭</span>
      <span class="bigfont">🤩</span>
      <span class="bigfont">😘</span>
  </header>

\--- /code ---

\--- /task ---

\--- task ---

Клацни на файл `animation.css` та знайди клас `bounceme`.

Анімація `bounce` має значення `ease`: вона плавно починається та закінчується, але прискорюється в середині.

## --- code ---

language: css
filename: animation.css
line_numbers: true
line_number_start: 17
line_highlights: 17-20
-----------------------------------------------------------

.bounceme {
animation: bounce ease 2s 3; /\* runs the 'bounce' animation with ease timing (slow start and end) for two seconds. Виконує анімацію тричі. \*/
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

**Поглянь:** властивість `scale` встановлює розмір, а властивість `translateY` рухає елемент вгору й униз за віссю y. Це створює ефект підстрибування.

\--- /task ---

\--- task ---

Клацни на файлі `index.html` та додай клас `bounceme` до емоджі з зірочками в очах 🤩.

## --- code ---

language: html
filename: index.html
line_numbers: true
line_number_start: 30
line_highlights: 35
--------------------------------------------------------

  <header class="secondary border-bottom">
    <h1>Пʼять найкращих емоджі!</h1>
    
    <span class="bigfont">🤣</span>
    <span class="bigfont">😇</span>
    <span class="bigfont">😭</span>
    <span class="bigfont bounceme">🤩</span>
    <span class="bigfont">😘</span>
  </header>

\--- /code ---

\--- /task ---

\--- task ---

**Протестуй:** натисни на кнопку **Run**.

Щоразу, коли ти завантажуєш сторінку, емоджі з зірочками 🤩 має підстрибнути тричі.

**Налагодження:**

\--- collapse ---

---

## title: Замість емоджі в заголовку підстрибує емоджі в списку!

Ти маєш додати `bounceme` до емоджі в заголовку `<header>`, а не до емоджі в списку `<ol>`.

\--- /collapse ---

\--- /task ---

Коли ти переглядаєш сторінку, її видима частина називається **полем перегляду**. Екран мобільного телефону має набагато менше поле перегляду, ніж екран комп'ютера.

У твоєму проєкті вже є код, який підлаштовує розмір та масштаб **поля перегляду** до ширини екрана конкретного пристрою. Ти можеш використовувати поле перегляду в анімаціях, щоб вони підлаштовували розмір відповідно до поля перегляду.

\--- task ---

Клацни на файл `animation.css` та знайди клас `rollmeleft`. Він створює анімацію, що викочується зліва.

Для створення ефекту перекочування використовується два оператори: `translate` та `rotate`.

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

**Поглянь:** Цей код `translate` використовує `vw` (viewport-width, з англійської «ширина поля перегляду»). Початкова точка `-60vw` знаходиться на 60% ліворуч від визначеної позиції у полі перегляду. Анімація закінчується у визначеній позиції `0vw`.

\--- /task ---

\--- task ---

Клацни на файлі `index.html` та додай клас `rollmeleft` (переворот ліворуч) до емоджі, що котиться по підлозі та сміється 🤣.

## --- code ---

language: html
filename: index.html
line_numbers: true
line_number_start: 30
line_highlights: 32
--------------------------------------------------------

  <header class="secondary border-bottom">
    <h1>Пʼять найкращих емоджі!</h1>
    
    <span class="bigfont rollmeleft">🤣</span>
    <span class="bigfont">😇</span>
    <span class="bigfont">😭</span>
    <span class="bigfont bounceme">🤩</span>
    <span class="bigfont">😘</span>
  </header>

\--- /code ---

\--- /task ---

\--- task ---

**Протестуй:** натисни на кнопку **Run**.

Емоджі, що котиться по підлозі та сміється 🤣, має викотитися з лівої частини екрану та обертатися під час руху.

**Порада:** натисни кнопку **Run**, щоб переглянути анімацію ще раз.

\--- /task ---

\--- task ---

**Вибір:** додай класи анімації до решти емоджі 😇😭😘, щоб надати своєму кумедному заголовку завершеного вигляду.

Ти можеш використовувати будь-які анімації з файлу `animation.css`:

- `spinme` (обертання)
- `bounceme` (підстрибування)
- `scaleme` (зміна розміру)
- `movemeleft` (рух ліворуч)
- `movemeright` (рух праворуч)
- `rollmeleft` (переворот ліворуч)
- `rollmeright` (переворот праворуч)

<div>
<iframe src="https://editor.raspberrypi.org/en/embed/viewer/top-5-emoji-list-step-6" width="500" height="500" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>

\--- /task ---
