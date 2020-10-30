# Marckdown

[Перейди что бы почитать про синтаксис подробнее](https://www.markdownguide.org/basic-syntax/)

**Markdown Preview Enhanced** [https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced)

Данный плагин позволит отображать то что мы пишем.

**Заголовки**

# Title

## Title

### Title

Some **text**, _italic_, ~~text~~,

```md
**text**, _italic_, ~~text~~,
```

## Links

1. https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced

<br>
<br>

2. [Текст какой-то](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced)
3. Ссылок может быть много поэтому их писать в таком формате бывает сложно. Что бы это упростить мы можем в самом конце файла в квадратных скобках определять либо цифрами **[1]** или названием или **[текстом]** далее пишу **:** и указываю ссылку. После чего я могу вместо ссылки спользовать этот ключ.

```md
<!-- Указываю текст и ключ -->

[Udemy](udemy)

<!-- Определяю в конце документа -->

[udemy]: https://www.udemy.com/

<!-- ключ может быть и цифрой -->
<!-- Указываю текст и ключ -->

[Udemy](1)

<!-- Определяю в конце документа -->

[1]: https://www.udemy.com/
```

<br>
<br>

## Images

![My image](https://unsplash.it/200/200)

И здесь я могу делать тоже самое что и со ссылками.

```md
![My image](random_image)

[random_image]: https://unsplash.it/200/200
```

<br>
<br>

## Lists

- List item 1
  - list item 1.1
    ![My image](https://unsplash.it/200/200)
- List item 2
- List item 3
- List item 4

<br>

1. List item 1
2. List item 2
3. List item 3

```md
- List item 1
  - list item 1.1
    ![My image](https://unsplash.it/200/200)
- List item 2
- List item 3
- List item 4

<br>

1. List item 1
2. List item 2
3. List item 3
```

<br>

## Lines

---

```md
--- три тере это горизонтальная линия
```

> Some text Для ответки важных частей документации.

<br>
<br>

## Code Block

```js
const a = 1;
```

inline code. Для этого обрамляю кавычками, не только к коду может применяться `пример`

```md
`пример`
```

Далее у нас есть отдельный блок кода для терминала ключевое слово **shell**

```shell
npm run dev
```

В блоке кода мы можем определить разницу между кодом. Ключевое слово **diff**

```diff
const a = 1;
- const y = 1;
+ const z = 1;
```

отмечается красным или зеленым как удаленные или добавленные части кода.

## Table

| Dir  |    Comment    |
| :--: | :-----------: |
| /src | some comments |
| /src | some comments |

```md
| Dir  |    Comment    |
| :--: | :-----------: |
| /src | some comments |
| /src | some comments |
```

Двоеточия используются для выравнивания текста. Два двоеточия это по цетру, по одному слева или справа соответсвенно выравнивание происходит по левому краю или по правому.

## TODO

- [x] Learn Java Script
- [ ] Learn React

```md
- [x] Learn Java Script
- [ ] Learn React
```
