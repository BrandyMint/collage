# Задача N1

## Написать функцию расстановки объектов в коллаж.

Аргументы:
* ширина контейнера (px)
* массив с объектами (количество объектов от 0 до 9)

У объектов три значения. width, height и payload.

Результат функции - массив строк.
Каждая строка из себя представляет массив смаштабированых объектов в таком порядке, чтобы они выстроились в коллаж (слева на право и с верху в низ)

## Пример вида коллажа

http://gyazo.com/aeb03a3dc86634511a67855192847e0a
Остюда: http://brandymint.github.io/mmm-tasty-static/tasty__tlog.html (попробуй туда повставлять несколько картинок, увидишь как коллаж с ними работает)

## Пример использования функции:

```
var images = [
{ width: 500, height: 900, payload: {} },
{ width: 100, height: 400, payload: {} },
{ width: 200, height: 300, payload: {} },
{ width: 300, height: 400, payload: {} },
{ width: 500, height: 900, payload: {} },
{ width: 100, height: 400, payload: {} },
{ width: 200, height: 300, payload: {} },
{ width: 300, height: 400, payload: {} }];

result = makeCollage(700, images);

result == [
[{ width: ?, height: ?, payload: {} },{ width: ?, height: ?, payload: {} },{ width: ?, height: ?, payload: {} },{ width: ?, height: ?, payload: {} }],
[{ width: ?, height: ?, payload: {} },{ width: ?, height: ?, payload: {} },{ width: ?, height: ?, payload: {} },{ width: ?, height: ?, payload: {} }]
]
```

## В помощь:

Вот плагин коллажа который у нас есть сейчас - https://github.com/BrandyMint/mmm-tasty-static/blob/develop/app/javascripts/old/plugins/jquery.collage.js

# Задача N2

Оформить задачу N1 в виде проекта для nodejs.

Для компиляции использовать grunt или gulp (он проще)

У этого проекда должно быть:

1. Каталог с исходником (src)
2. Компиляция исходника в минимизированном виде в (dist)
3. Тесты для количества картинок от 0 до 4.


## Пример

на grunt https://github.com/mduvall/grande.js
