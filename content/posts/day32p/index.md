---
title: "Day32"
date: 2023-12-01T09:51:21+03:00
image: "Day-32.png"
draft: false
tags:
- практика
---


- [X] Kata
- [X] Journey
- [ ] Theory
- [ ] Practice
- [ ] Schedule

# Kata

5 kyu: https://www.codewars.com/kata/52bc74d4ac05d0945d00054e/train/javascript

Я вас категорически приветствую.

Мое решение:

```js
function firstNonRepeatingLetter(s) {

    for (let letter of s) {
        let obviousCount = countChar(s, letter);
        let transformedCount = countChar(s, transform(letter));
        if (letter === transform(letter)) {
            transformedCount --;
        }
        if ( obviousCount + transformedCount > 1) {
        } else {
            return letter;
        }
    }
    return '';
}

function transform(ch) {
    if (ch === ch.toUpperCase()) {
        return ch.toLowerCase();
    } else {
        return ch.toUpperCase();
    }
}

function countChar(str, ch) {
    let count = 0;
    for(let i= 0; i < str.length; i += 1) {
        if (str.charAt(i) === ch) {
            count++;
        }
    }
    return count;
}

```

Идеальное не буду скидывать, так как я его не нашел(или просто стыдно) (