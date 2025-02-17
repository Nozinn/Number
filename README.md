# Number
# Number в JavaScript

`Number` — это примитивный тип данных в JavaScript, используемый для представления чисел, включая целые и дробные значения.

## Основные особенности
- Использует стандарт IEEE 754 (64-битное представление).
- Поддерживает целые числа, числа с плавающей запятой и специальные значения (`Infinity`, `-Infinity`, `NaN`).
- Для работы с большими числами можно использовать `BigInt`.

## Специальные значения
- `Infinity` и `-Infinity` — бесконечные значения, возникающие при переполнении.
- `NaN` (Not-a-Number) — результат некорректных математических операций.

## Методы объекта Number
```js
(3.14159).toFixed(2); // "3.14"
(123.456).toPrecision(4); // "123.5"
(255).toString(16); // "ff"
```

## Проверка чисел
```js
Number.isNaN(0 / 0); // true
Number.isFinite(100); // true
Number.isInteger(42); // true
```

## Границы значений
```js
console.log(Number.MAX_SAFE_INTEGER); // 9007199254740991
console.log(Number.MIN_SAFE_INTEGER); // -9007199254740991
```

### Работа с `BigInt`
```js
let big = 9007199254740991n;
console.log(big + 1n); // 9007199254740992n
```

### Дополнительная информация
Полная документация доступна на [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number).

