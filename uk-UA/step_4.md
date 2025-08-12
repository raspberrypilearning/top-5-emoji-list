## Додай фонове зображення

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">

Додай барвисте тло з емоджі та зроби основну частину сторінки прозорою, щоби фонове зображення було видно крізь основний вміст.

</div>
<div>
<iframe src="https://editor.raspberrypi.org/uk-UA/embed/viewer/top-5-emoji-list-step-4" width="500" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>
</div>

Властивість CSS `background-image` дозволяє встановити зображення як фон для вебсторінки.

--- task ---

**Знайди** у файлі `style.css` правило CSS `body` та **розкоментуй** рядок `background-image`, щоб встановити фонове зображення для своєї сторінки.

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 44
line_highlights: 47
---
\*додай фонове зображення до основної частини */

body {
  background-image: url('emojis.png'); /* Прибери позначки коментаря і зміни назву файлу, щоб додати фонове зображення
  /*background-repeat: repeat;*/ /* Зроби зображення повторюваним */
  /*background-size: cover;*/ /* Зроби так, щоб зображення заповнило весь контейнер */
}

--- /code ---

--- /task ---

--- task ---

**Протестуй:** натисни на кнопку **Run**.

Ти маєш побачити барвисті зображення емоджі по краях своєї сторінки.

**Порада:** щоби переглянути фонове зображення, тобі може знадобитися ширша область виводу.

**Порада:** якщо ти переглядаєш сторінку на мобільному телефоні, поверни екран в альбомний режим.

--- /task ---

**Непрозорість** означає, наскільки добре видно крізь елемент. Якщо непрозорість дорівнює 1, то HTML-елемент є суцільним, і крізь нього нічого не видно. Якщо непрозорість дорівнює 0, то елемент повністю прозорий.

--- task ---

**Знайди** у файлі `style.css` коментар `/* Додай ефект прозорості */`.

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 93
line_highlights: 93
---

\*Додай ефект прозорості */

--- /code ---

--- /task ---

Досі ми використовували класи CSS, які були створені спеціально для цього проєкту. Тепер ти самостійно створиш новий CSS-клас під назвою `transparent`, за допомогою якого можна зробити HTML-елемент `<main>` прозорим.

Значення непрозорості (opacity) в `0.95` означає, що елемент трохи прозорий.

Додай правило `.transparent` під коментарем.

--- task ---

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 93
line_highlights: 95-97
---

\*Додай ефект прозорості */

.transparent {
 opacity: 0.95;
}

--- /code ---

--- /task ---

Тепер ти маєш застосувати щойно створений CSS-клас.

--- task ---

Додай свій новий клас `transparent` до секції `<main>` у HTML-файлі.

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

**Протестуй:** натисни на кнопку **Run**.

Переконайся, що основна частина твоєї сторінки трохи прозора.

Що станеться, якщо змінити значення `opacity` на `0.50`, `0.75` або `0.90`? Спробуй використати різні значення у своєму CSS-правилі та вибери, яке тобі більше подобається.

<div>
<iframe src="https://editor.raspberrypi.org/uk-UA/embed/viewer/top-5-emoji-list-step-4" width="500" height="700" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen> </iframe>
</div>

--- /task ---
