# 📌 Числа (Number) в JavaScript

В JavaScript тип `Number` используется для работы с числами (целыми и десятичными). 

---

## 🔢 Основные особенности:
✅ Числа в JavaScript используют стандарт **IEEE 754 (64-битное представление)**.  
✅ Можно работать с **целыми** и **дробными** числами.  
✅ Есть специальные значения: `Infinity`, `-Infinity`, `NaN`.  
✅ Если нужны большие числа, можно использовать `BigInt`.

---

## 🏆 Основные методы `Number`

### 🔹 `toFixed(n)` – округление до `n` знаков после запятой
```js
let num = 3.14159;
console.log(num.toFixed(2)); // "3.14"
```
📌 Используется, когда нужно ограничить количество знаков после запятой.

### 🔹 `toPrecision(n)` – представление числа с `n` значащими цифрами
```js
let num = 123.456;
console.log(num.toPrecision(4)); // "123.5"
```
📌 Полезно, когда нужно контролировать общее количество цифр в числе.

### 🔹 `toString(radix)` – перевод числа в строку с нужной системой счисления
```js
let num = 255;
console.log(num.toString(16)); // "ff" (шестнадцатеричное представление)
console.log(num.toString(2));  // "11111111" (двоичное представление)
```
📌 Можно преобразовать число в **двоичный, восьмеричный, шестнадцатеричный** формат.

---

## ❓ Проверка чисел

### ✅ `Number.isNaN(value)` – проверка, является ли значение `NaN`
```js
console.log(Number.isNaN(0 / 0)); // true
console.log(Number.isNaN("hello")); // false
```
📌 `NaN` возникает при некорректных математических операциях.

### ✅ `Number.isFinite(value)` – проверка, является ли число конечным
```js
console.log(Number.isFinite(100)); // true
console.log(Number.isFinite(Infinity)); // false
```
📌 Полезно, чтобы избежать ошибок при работе с большими числами.

### ✅ `Number.isInteger(value)` – проверка, является ли число целым
```js
console.log(Number.isInteger(42)); // true
console.log(Number.isInteger(3.14)); // false
```
📌 Отлично подходит для проверки, является ли число **целым**.

---

## 📏 Границы значений

| Свойство | Значение |
|----------|----------|
| `Number.MAX_SAFE_INTEGER` | 9007199254740991 |
| `Number.MIN_SAFE_INTEGER` | -9007199254740991 |
| `Number.EPSILON` | 2.220446049250313e-16 |

📌 **`MAX_SAFE_INTEGER`** – максимальное безопасное целое число в JS.
📌 **`EPSILON`** – минимальная разница между двумя числами.

---

## 🔥 Работа с `BigInt`
`BigInt` используется для работы с очень большими числами.
```js
let big = 9007199254740991n;
console.log(big + 1n); // 9007199254740992n
```
📌 Обрати внимание на **`n`** в конце числа – оно обозначает `BigInt`.

---

## 📚 Дополнительная информация
📖 Полная документация на [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number).

![JavaScript Numbers](https://upload.wikimedia.org/wikipedia/commons/6/6a/JavaScript-logo.png)

 😊

