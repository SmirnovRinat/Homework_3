# Создание справки по системе контроля версий GIT


## Как начать?
**Чтобы начать работать с системой контроля версий Git, необходимо выполнить следующую команду:**

```cs
git init
```

## Как добавить файл в отслеживание

**Чтобы добавить файл в отслеживание, используйте команду:**

```
git add namefile
```

или

```
git add .
```
**Чтобы получить информацию от git о его текущем состоянии, используйте команду:**

```
git status
```

**Чтобы создать коммит, используйте команду:**

```
git commit -m “message”
```

**Чтобы вывести на экран истории всех коммитов с их хеш-кодами, используйте команду:**

```
git log
```


**Чтобы перейти от одного коммита к другому, используйте команду:**

```
git checkout
```


# Создание руководства по языку разметки MarkDawn


## Создание заголовков




## Добавление изображений

Чтобы добавить изображения, можно воспользоваться следующими конструкциями:

Картинка без `alt` текста

![](https://static.wikia.nocookie.net/pogod/images/3/3a/%D0%9F%D1%80%D0%B8%D1%80%D0%BE%D0%B4%D0%B0.jpg/revision/latest/scale-to-width-down/1200?cb=20181224151953&path-prefix=ru)

Картинка с альтом и тайтлом:

![Alt text](https://static.wikia.nocookie.net/pogod/images/3/3a/%D0%9F%D1%80%D0%B8%D1%80%D0%BE%D0%B4%D0%B0.jpg/revision/latest/scale-to-width-down/1200?cb=20181224151953&path-prefix=ru "Можно задать title")

Запомнить просто: синтаксис как у ссылок, только перед открывающей квадратной скобкой ставится восклицательный знак.

Картинки «сноски»:

![Картинка](https://static.wikia.nocookie.net/pogod/images/3/3a/%D0%9F%D1%80%D0%B8%D1%80%D0%BE%D0%B4%D0%B0.jpg/revision/latest/scale-to-width-down/1200?cb=20181224151953&path-prefix=ru)
![Картинка][image2]
![Картинка][image3]

[image1]: //placehold.it/250x100
[image2]: //placehold.it/200x100
[image3]: //placehold.it/150x100

Картинки-ссылки:

[![Alt text](https://static.wikia.nocookie.net/pogod/images/3/3a/%D0%9F%D1%80%D0%B8%D1%80%D0%BE%D0%B4%D0%B0.jpg/revision/latest/scale-to-width-down/1200?cb=20181224151953&path-prefix=ru)](https://www.youtube.com/watch?v=ccUr2giQI0M&ab_channel=DimitriDumas)





## Добавление исходного кода 

В чистом Маркдауне блоки кода отбиваются 4 пробелами в начале каждой строки.

Но в GitHub-Flavored Markdown (сокращенно GFM) есть более удобный способ: ставим по три апострофа (на букве Ё) до и после кода. Также можно указать язык исходного кода.

```python
@route("/")
def start():
    return renderer("index.html")
```







## Добавление таблиц


В чистом Маркдауне нет синтаксиса для таблиц, а в GFM есть.

First Header  | Second Header
------------- | -------------
Content Cell  | Content Cell
Content Cell  | Content Cell

Для красоты можно и по бокам линии нарисовать:

| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

Можно управлять выравниванием столбцов при помощи двоеточия.

| Left-Aligned  | Center Aligned  | Right Aligned |
|:------------- |:---------------:| -------------:|
| col 3 is      | some wordy text |     **$1600** |
| col 2 is      | centered        |         $12   |
| zebra stripes | are neat        |        ~~$1~~ |

Внутри таблиц можно использовать ссылки, наклонный, жирный или зачеркнутый текст.

Для всего остального есть обычный HTML.

## Списки
Для разметки неупорядоченных списков можно использовать или `*`, или `-`, или `+`:

- элемент 1
- элемент 2
- элемент ...

Вложенные пункты создаются четырьмя пробелами перед маркером пункта:

* элемент 1
* элемент 2
    * вложенный элемент 2.1
    * вложенный элемент 2.2
* элемент ...

Упорядоченный список:

1. элемент 1
2. элемент 2
    1. вложенный
    2. вложенный
3. элемент 3
4. Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse id sem consectetuer libero luctus adipiscing.

На самом деле не важно как в коде пронумерованы пункты, главное, чтобы перед элементом списка стояла цифра (любая) с точкой. Можно сделать и так:

0. элемент 1
0. элемент 2
0. элемент 3
0. элемент 4

Список с абзацами:

* Раз абзац. Lorem ipsum dolor sit amet, consectetur adipisicing elit.

* Два абзац. Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse id sem consectetuer libero luctus adipiscing.

* Три абзац. Ea, quis, alias nobis porro quos laborum minus sed fuga odio dolore natus quas cum enim necessitatibus magni provident non saepe sequi?

    Четыре абзац (Четыре пробела в начале или один tab).

## Цитаты


## Горизонтальная черта


## Зачеркивание