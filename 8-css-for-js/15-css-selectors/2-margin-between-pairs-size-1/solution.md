# Выбор элементов

Для выбора элементов, начиная с первого, можно использовать селектор [nth-child](http://css-tricks.ru/Articles/Details/HowNthChildWorks).

Его вид: `li:nth-child(n+2)`, т.к. `n` идёт от нуля, соответственно первым будет второй элемент (`n=0`), что нам и нужно.

# Решение

Отступ, размером в одну строку, при `line-height: 1.5` -- это `1.5em`.

Правило:

```css
li:nth-child(n+2) {
  margin-top: 1.5em;
}
```

# Ещё решение

Ещё один вариант селектора: `li + li`

```css
li + li {
  margin-top: 1.5em;
}
```

