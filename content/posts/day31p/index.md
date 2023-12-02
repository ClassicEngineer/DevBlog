---
title: "Day31p"
date: 2023-11-30T08:46:55+03:00
image: "snow-city.gif"
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

5 kyu: https://www.codewars.com/kata/520b9d2ad5c005041100000f/javascript

И снова здравствуйте.

Мое решение: 

```js
let pigIt = (str) => {
    let result = '';
    let words = [];
    let regexp = RegExp('[a-zA-Z]+', 'g');
    let regExpArray;
    let word = '';
    do  {
        regExpArray = regexp.exec(str);
        if (regExpArray) {
            word = regExpArray[0];
            words.push({word: word, index: regExpArray.index});
        }
    } while (regExpArray)

    for (let i = 0; i < words.length; i++) {
        let replace = words[i].word.substring(1) + words[i].word[0] + 'ay';
        let nextWordIndex = i === words.length - 1 ?  str.length : words[i+1].index;
        let nonWordsSymbols = str.substring(words[i].index + words[i].word.length, nextWordIndex);
        result += replace + nonWordsSymbols;
    }
    return result;
}

```

Идеальное решение :

```js
function pigIt(str){
    return str.replace(/(\w)(\w*)(\s|$)/g, "\$2\$1ay\$3")
}
```


#JOURNEY
Кодил много по проекту. Жаль что гихтаб коммиты не показывает в зеленых квадратиках.

# Today I learned

функции в JavaScript — это объекты первого класса, что позволяет использовать их как функции высшего порядка и возвращать из них другие функции.