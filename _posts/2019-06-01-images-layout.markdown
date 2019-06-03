---
layout: post
title:  "Верстка картинок"
date:   2019-06-01 19:21:59 +0300
categories: front-end images
---

Чтобы картинка всегда помещалась в контейнер и ужималась при необходимости

```
img {
  max-width: 100%;
  height: auto;
}
```

Чтобы не было расстояния между картинкой и нижней границей контейнера, у контейнера надо обнулить шрифт

```
<container>
  <img src="https://dummyimage.com/600x400/ffff77/00ffd9.jpg">
</container>
```

```
container {
  border: 1px solid black;
  font-size: 0;
}
```
Свойство [object-fit](https://developer.mozilla.org/en-US/docs/Web/CSS/object-fit) позволяет использовать разные способы подгонки картинки под размер контейнера.

[Полифилл для IE11](https://codepen.io/jonneal/pen/EKPONK)