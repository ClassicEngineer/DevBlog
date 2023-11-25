---
title: "Day 27"
date: 2023-11-25T14:42:25+03:00
image: "anime_snow.webp"
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

Посчитал биты : https://www.codewars.com/kata/526571aae218b8ee490006f4/solutions/javascript

```js

function dec2bin(dec) {
    return dec.toString(2);
}

function countChar(str, ch) {
    let count = 0;
    for(let i=0; i < str.length; i += 1) {
        if (str.charAt(i) === ch) {
            count++;
        }
    }
    return count;
}
var countBits = function(n) {
    const bin = dec2bin(n);
    return countChar(bin, '1');
};


```

# Theory

Теория гридов

# Practice

- Поверстал простейший сайт-портфолио.
- Прошел до конца курс [JavaScript для начинающих](https://stepik.org/course/2223)
- Попрактиковался в гридах

# Journey

Собираюсь посмотреть https://www.youtube.com/watch?v=GNrdg3PzpJQ

# Итого

Хороший день. Указанное выше видео очень порадовало. С его помощью я гораздо быстрее разберусь с  React и начну писать свои проекты на нем. 

# Разное

# Today I learned

Замыкания, RegExp в JS, побольше про раскладку гридами.