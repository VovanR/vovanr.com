```
title: Photoshop экшены для верстальщика
layout: post
tags:
  - 'photoshop'
  - 'actions'
date: 2013-03-03
```

Рассмотрим полезные экшены (проще говоря макросы) *Photoshop* для облегчения работы верстальщика с макетами.

Какие действия мы делаем чаще всего? Режем!

[Скачать экшены](https://yadi.sk/d/Zf1e4V5y30B_x)


### Обрезаем прозрачные области картинки

![Подготовка картинки с прозрачным фоном](/images/photoshop-actions/photoshop-actions__action-1.png)

<kbd>Image</kbd>→<kbd>Trim...</kbd>

```nohighlight
Based On: Transparent Pixels
Trim Away: Top, Left, Bottom, Right
```


### Обрезаем однотонные области картинки <small>(например иконка на белом фоне)</small>

![Подготовка картинки с цветным фоном](/images/photoshop-actions/photoshop-actions__action-2.png)

<kbd>Image</kbd>→<kbd>Trim...</kbd>

```nohighlight
Based On: Bottom Right Pixel Color
Trim Away: Top, Left, Bottom, Right
```


### Для вертикального градиента делаем ширину `1px`

![Подготовка градиента](/images/photoshop-actions/photoshop-actions__action-3.png)

<kbd>Image</kbd>→<kbd>Canvas Size...</kbd>

Снимаем галку `Relative`, в поле `Width` пишем `1`.

<p class="special"><strong>Совет:</strong> помните, что дешевле всего вертикальные градиенты хранить в <code>PNG-24</code></p>
