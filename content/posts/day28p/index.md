---
title: "Day 28"
date: 2023-11-26T12:36:37+03:00
image: "snow-winter.gif"
draft: false
tags:
- практика
---


- [X] Kata
- [X] Theory
- [X] Practice
- [X] Journey
- [X] Schedule


# Kata

6 kyu: https://www.codewars.com/kata/550498447451fbbd7600041c/solutions/javascript

```js

function comp(array1, array2){
    if (array1 == null && array2 == null) {
        return true
    } else if (array1 == null || array2 ==null) {
        return false;
    }
    for (let i = 0; i <array2.length; i++) {
        let a2sqr = Math.sqrt(array2[i]);
        if (array1.indexOf(a2sqr) < 0) {
            return false;
        } else {
            array1[array1.indexOf(a2sqr)] = null;
        }
    }
    return true;
}

```

# Theory

Теория слекторов и работы с иконками и изображениями
Досмотрел React от A до Я. Мощно. Очень мощно. Сразу все не понятно, но очень даже применимо и увлекательно.


# Practice

Практика верстки простейшего Портфолио


# Journey

Заметил, что откладываю "Путешествие" aka свой проект на конец дня. Когда уже не остается сил на героические совершения.
Да, самому с нуля разрабатывать это сложно, но это разиввает больше всего. Перенесу в начало дня.

Начал пилить бэкенд блога.

# Итого


# Разное

