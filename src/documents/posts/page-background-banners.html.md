```
title: Баннеры на фоне сайта
layout: post
tags:
  - 'css'
  - 'html'
date: 2012-08-07
```

![](/images/page-background-banners/page-background-banners__preview.png)

Как поставить баннеры на фон страницы сайта? Без горизонтальной прокрутки? Элементарно: [пример](https://jsfiddle.net/VovanR/k9wec/2/).

**CSS:**

```css
body {
  color: #000;
  font: 0.8em "Arial", "Helvetica", sans-serif;
  background: #FFF;
  margin: 0;
  padding: 0 0 1em;
  position: relative;
  z-index: 0;
}
.page {
  background: #445A71;
  min-width: 300px;
  margin: 0;
  padding: 0;
}
.page_banner_ru {
  background: #0C1D63;
}

.wrotator {
  text-align: center;
  width: 100%;
  height: 500px;
  position: absolute;
  z-index: 1;
  overflow: hidden;
}
  .wrotator__i {
    min-width: 300px;
    max-width: 400px;
    margin: 0 auto;
    position: relative;
  }
    .wrotator__left {
      width: 200px;
      height: 500px;
      position: absolute;
      left: -200px;
    }
    .page_banner_ru .wrotator__left {
      background: transparent url("https://placehold.it/100x500/f8abe1/fff&text=BANNER") 100% 0 no-repeat;
    }
    .wrotator__right {
      width: 200px;
      height: 500px;
      position: absolute;
      right: -200px;
    }
    .page_banner_ru .wrotator__right {
      background: transparent url("https://placehold.it/100x500/f8abe1/fff&text=BANNER") no-repeat;
    }

.l-width__i {
  max-width: 400px;
  min-width: 300px;
  margin: 0 auto;
  background: #FFF;
  position: relative;
  z-index: 2;
}
```

**HTML:**

```html
<!--
Баннеры по бокам страницы
Скопипащено с яндекса (http://football2012.yandex.ru/)
-->
<!DOCTYPE html>
<html>
<head>
  <title>Баннеры по бокам страницы</title>
  <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
</head>
<body class="page page_banner_ru">

<div class="wrotator">
  <div class="wrotator__i">
    <!-- Баннер слева -->
    <a class="wrotator__left" href="https://ya.ru/" target="_blank"></a>

    <!-- Баннер справа -->
    <a class="wrotator__right" href="https://ya.ru/" target="_blank"></a>
  </div>
</div>

<div class="l-width">
  <div class="l-width__i">
    <div class="l-width__i__i">

      <!-- Здесть контент страницы -->
      <p>Content there</p>

    </div>
  </div>
</div>

</body>
</html>
```
