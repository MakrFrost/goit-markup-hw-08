# goit-markup-hw-08

https://makrfrost.github.io/goit-markup-hw-08/

Игорёха, это АД

```css
<!--  Для рассчёта карточек в ряд (для адаптива и не только) -->
<!-- Задаем фикс отступ в виде переменной -->
:root{
--gap-card: 30px
}


<!-- Список -->
&-list {
<!-- Ставит в ряд -->
display: flex;
flex-wrap: wrap;
<!-- Центрирует -->
justify-content: center;
<!-- Задает отрицательный марджин -->
margin-top: calc(-1 * var(--gap-card));
margin-left: calc(-1 * var(--gap-card));
}

<!-- Карточка -->
&__item {
<!-- Задает количество карточеку в ряду, зависимо от того сколько их там нужно -->
flex-basis: calc(100% / 2 - var(--gap-card));
margin-top: var(--gap-card);
margin-left: var(--gap-card);
<!-- Убирает ненужное -->
&:not(:last-child) {
margin-bottom: 0;
}
}
```
