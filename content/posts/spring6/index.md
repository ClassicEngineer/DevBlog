---
title: "Что новенького в Spring 6"
date: 2023-07-05T15:52:24+03:00
image: "NewInSpring6.webp"
draft: false
# tags:
#   - tagA
#   - tagB
---



Вольный и упрощенный перевод с https://www.baeldung.com/spring-boot-3-spring-6-new

##  1. Java 17 - Основной язык


### Что новенького в самой Java 17


### 1.1. Records


Мы легко можем создавать неизменяемые DTO's

```java
public record Person (String name, String address) {}
```


### 1.2. Text Blocks



C [JEP 378](https://openjdk.java.net/jeps/378), теперь возможно создавать multi-line текстовые блоки

```java
String textBlock = """
Hello, this is a
multi-line
text block.
""";
```

### 1.3. Switch Expressions


Новый switch-case

```java
DayOfWeek day = DayOfWeek.FRIDAY;
int numOfLetters = switch (day) {
    case MONDAY, FRIDAY, SUNDAY -> 6;
    case TUESDAY                -> 7;
    case THURSDAY, SATURDAY     -> 8;
    case WEDNESDAY              -> 9;
};
```

### 2.4. Pattern Matching


Матчинг объектов по классу.

Напрямую в  _instanceof_:

```java
if (obj instanceof String s) {
    System.out.println(s.toLowerCase());
}
```

Или в _switch_–_case_ конструкции:

```java
static double getDoubleUsingSwitch(Object o) {
    return switch (o) {
        case Integer i -> i.doubleValue();
        case Float f -> f.doubleValue();
        case String s -> Double.parseDouble(s);
        default -> 0d;
    };
}
```

### 2.5. Sealed Classes and Interfaces


Sealed classes могут наследовать только опредлённые указанные классы:

```java
public abstract sealed class Pet permits Dog, Cat {}
```



## 3. Jakarta EE 9


Самое основное изменение это переход с Java EE к Jakarta EE9, где пакеты namespace поменяются с _javax.*_ на  _jakarta.*_. 

Например:

```java
import javax.servlet.http.HttpServletRequest;
```

Надо заменить на:

```java
import jakarta.servlet.http.HttpServletRequest;
```


## 4. Новые версии зависимостей


Spring Framework 6 и Spring Boot 3 теперь нужны следующие минимальные версии:

- Kotlin 1.7+
- Lombok 1.18.22+ 
- Gradle 7.3+

## 5. Основные изменения

_Native Executables_ И _Observability_. 

### 5.1. Native Executables

Возможность исполнять нативный код

Пример для AOT generation в Maven :

```bash
mvn spring-boot:aot-generate
```



### 5.2. Observability

Spring 6 представляет [Spring Observability](https://spring.io/blog/2022/10/12/observability-with-spring-boot-3) – новая инициатива построенная на Micrometer и Micrometer Tracing. Цель - снимать метрики с приложения более эффективно

## 6. Маленькие изменения в Spring Web MVC

- [support for RFC7807](https://github.com/spring-projects/spring-framework/issues/27052)
- HttpMethod больше не Enum
* улучшена загрузка файлов ( [_StandardServletMultipartResolver_](https://www.logicbig.com/tutorials/spring-framework/spring-web-mvc/file-upload-servlet-resolver.html) )
* поддержка Tiles и FreeMarker JSP .

### Итог

Изменилось многое, но надо смотреть детальней чтобы это понять.