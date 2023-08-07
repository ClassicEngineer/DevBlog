---
title: "Пишем свой Spring Boot Starter"
date: 2023-08-03T10:06:37+03:00
image: "starter.jpg"
draft: false
tags:
- tech

---

В целом нужно два файла:


`META-INF/spring.factories`

```java

org.springframework.boot.autoconfigure.EnableAutoConfiguration=\
path.to.your.XAutoConfiguration

```
И собственно сам `XAutoConfiguration`
```java

@Configuration
public class XAutoConfiguration {...}

```

Все остальное по желанию и потребностям.

Далее требуется объединить два моудля с помощью maven или gradle. И вуаяля, стартуем!


![](start.jpg)

Но в реальности что-то не всегда стартует. Надо разобраться почему