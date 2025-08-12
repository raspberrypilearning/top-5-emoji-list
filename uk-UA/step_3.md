## Створи анімацію емоджі

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
На цьому кроці ти додаси до своєї сторінки велике анімоване емоджі, щоб зробити її цікавішою для відвідувачів.
</div>
<div>
<iframe src="https://editor.raspberrypi.org/uk-UA/embed/viewer/top-5-emoji-list-step-3" width="500" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>
</div>

--- task ---

Ти використаєш велике емоджі трофея, яке означатиме, що це найпопулярніші емоджі.

Додай новий абзац за допомогою тегу `<p>` до своєї секції (`<section>`) і розмісти там емоджі 🏆.

Клас `hugefont` робить текст з емоджі величезним!

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
          <li>🤣 – катаюсь по підлозі від сміху.</li>
          <li>👍👍🏻👍🏼👍🏽👍🏾👍🏿 – великий палець догори.</li>
          <li>😭 – голосно плачу.</li>
          <li>🙏🙏🏻🙏🏽🙏🏽🙏🏾🙏🏿 – складені долоні.</li>
          <li>😘 – шлю поцілунок.</li>
        </ol>
        <p class="hugefont">🏆</p>  
      </section>

--- /code ---

--- /task ---

--- task ---

**Протестуй:** натисни на кнопку **Run**.

Подивись, чи з'являється під списком великий емоджі-трофей.

--- /task ---

--- task ---

Додай клас `wrap` до секції `<section>`, щоб зробити свій вебсайт більш адаптивним. Цей клас буде налаштовувати макет відповідно до розміру екрану.

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
          <li>🤣 – катаюсь по підлозі від сміху.</li>
          <li>👍👍🏻👍🏼👍🏽👍🏾👍🏿 – великий палець догори.</li>
          <li>😭 – голосно плачу.</li>
          <li>🙏🙏🏻🙏🏽🙏🏽🙏🏾🙏🏿 – складені долоні.</li>
          <li>😘 – шлю поцілунок.</li>
        </ol>
        <p class="hugefont">🏆</p>  
      </section>

--- /code ---

--- /task ---

--- task ---

**Протестуй:** натисни на кнопку **Run**.

Перевір, чи відображається трофей наступним у списку, якщо сторінка достатньо широка. Список і трофей повинні мати однакову ширину.

--- /task ---

Таблиця стилів також містить класи `wide` та `narrow`, які можна використовувати для зміни ширини різних елементів:

- Додай клас `wide` до тегу `<ol>`.

- Додай клас `narrow` до абзацу з емоджі-трофеєм.

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
          <li>🤣 – катаюсь по підлозі від сміху.</li>
          <li>👍👍🏻👍🏼👍🏽👍🏾👍🏿 – великий палець догори.</li>
          <li>😭 – голосно плачу.</li>
          <li>🙏🙏🏻🙏🏽🙏🏽🙏🏾🙏🏿 – складені долоні.</li>
          <li>😘 – шлю поцілунок.</li>
        </ol>
      <p class="hugefont narrow">🏆</p>     
      </section>

--- /code ---

--- /task ---

--- task ---

**Протестуй:** натисни на кнопку **Run**.

Подивись, чи став список ширшим. Якщо твоя сторінка достатньо широка, трофей буде видно праворуч.

--- /task ---

Ти також можеш використовувати HTML та CSS для створення **анімацій**, які змінюють елементи на вебсторінці.

Правило CSS `@keyframes` (ключові кадри) можна налаштувати так, щоб вони змінювалися з часом. Можна змінювати колір, положення, розмір та тип обертання елемента, а також багато інших властивостей.

Правило `@keyframes` контролює вигляд елементу після виконання певного відсотка анімації.

--- task ---

**Знайди** клас `.spinme` на початку файлу `animation.css`. Ми створили клас `.spinme` спеціально для цього проєкту. Він запускає CSS-анімацію під назвою `rotate-center`, яка обертає елемент від початкової позиції в 0 градусів і до 360 градусів.

Рядок `animation: rotate-center linear 8s 2;` каже класу використовувати анімацію `rotate-center` з лінійною тривалістю, тобто з однаковою швидкістю увесь час. Анімація триває вісім секунд і повторюється двічі.

--- code ---
---
language: CSS
filename: animation.css
line_numbers: true
line_number_start: 1
line_highlights: 1-4
---
.spinme {
  animation: rotate-center linear 8s 2; /* Тривалість анімації та кількість повторень */
  display: inline-block;
}

@keyframes rotate-center {
  /* Код анімації rotate */
  0% { 
    /* Обертання від 0 до 360 градусів */
    transform: rotate(0);
  }
  100% {
    transform: rotate(360deg);
  }
}
 
--- /code ---

--- /task ---

--- task ---

Повернися до файлу `index.html`.

Додай клас `spinme` до абзацу з трофеєм.

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
                <li>🤣 – катаюсь по підлозі від сміху.</li>
                <li>👍👍🏻👍🏼👍🏽👍🏾👍🏿 – великий палець догори.</li>
                <li>😭 – голосно плачу.</li>
                <li>🙏🙏🏻🙏🏽🙏🏽🙏🏾🙏🏿 – складені долоні.</li>
                <li>😘 – шлю поцілунок.</li>
            </ol>
            <p class="hugefont narrow spinme">🏆</p>         
        </section>

--- /code ---

--- /task ---

--- task ---

**Протестуй:** натисни на кнопку **Run**.

Твій трофей має обертатися двічі щоразу, коли ти завантажуєш сторінку (кнопкою **Run**).

--- /task ---

--- task ---

Повернися до файлу `animation.css`.

**Вибери:** Зміни два останні значення в рядку `animation: rotate-center linear 8s 2;` на свій смак.

- Що станеться, якщо виконувати анімацію понад вісім секунд?
- Ти хочеш, щоб анімація виконувалася більше двох разів?

<iframe src="https://editor.raspberrypi.org/uk-UA/embed/viewer/top-5-emoji-list-step-3" width="600" height="700" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>

--- /task ---


