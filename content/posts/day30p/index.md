---
title: "Day30p"
date: 2023-11-28T10:07:58+03:00
image: "snow-road.webp"
draft: false
tags:
- практика
---


- [X] Kata
- [X] Journey
- [ ] Theory
- [X] Practice
- [ ] Schedule

# Kata

6 kyu: https://www.codewars.com/kata/585d7d5adb20cf33cb000235/solutions/javascript

```js
function findUniq(arr) {
    let num = arr[0];
    if (num != arr[1]) {
        return num === arr[2] ? arr[1] : num; 
    }
    for(let i = 0; i < arr.length; i++) {
        if (arr[i] !== num) {
            return arr[i];
        }
    }
    return arr[0];
}

```

# Journey

Н-да. Вроде программирую уже больше 5 лет.
А как сделать какие-то казалось бы простые вещи вроде текстового редактора не знаю.
Иногда это расстраивает. Но в конечном итоге, понимаю, что все это такая фигня. Разработка, бэкенд, фронтенд..
Можно использовать громкие слова типа инженерия, исскуство, самовыражение, ремесло..дело всей жизни и прочее прочее...
Но это не отменяет того факта, что все это пусто само по себе.Нравится - делаешь. Не нравится - не делаешь.
