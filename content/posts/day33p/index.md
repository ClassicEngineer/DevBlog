---
title: "Day33"
date: 2023-12-02T12:18:12+03:00
image: "Day-33.png"
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

5 kyu: https://www.codewars.com/kata/515bb423de843ea99400000a/solutions/javascript

Всем привет.

Мое решение:


```js
class PaginationHelper {
    constructor(collection, itemsPerPage) {
        this.itemsPerPage = itemsPerPage;
        this.items = collection.length;
        this.pages = Math.ceil(this.items /this.itemsPerPage);

    }
    itemCount() {
        return this.items;
    }
    pageCount() {
        return this.pages;
    }

    pageItemCount(pageIndex) {
        if (pageIndex >= this.pages) {
            return  -1;
        }
        let skip = pageIndex * this.itemsPerPage;
        let remain = this.items - skip;
        return (remain / this.itemsPerPage) > 1 ? this.itemsPerPage: remain;
    }

    pageIndex(itemIndex) {
        if (itemIndex < 0 ||itemIndex >= this.items) {
            return -1;
        }
        return Math.floor(itemIndex / this.itemsPerPage);
    }
}

```

# Journey

Писал что-то для блога..