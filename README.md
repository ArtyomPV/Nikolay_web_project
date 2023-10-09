1. тег body был внутри тега head
2. Использованы абсолютные пути, а нужны относительные пути (относительно того где расопложен файл, в данном случае index.html)
Стили у меня не заработали, так как по тому пути, что указано у меня файла нет, используем относительный путь
```
<!--            <link rel="stylesheet" href="C:\Users\User\Desktop\Programming\html\project1\CSS\style.css"> -->
    <link rel="stylesheet" href="./CSS/style.css">
```
```html
<a href="C:\Users\User\Desktop\Programming\html\project1\index.html" class="logo_link">-->
                    
```
нужно прописать в таком виде
```html
<a href="index.html" class="logo_link">
```

у тебя основной контент разделен на несколько секций, лучше разбить body на  section

```html
<body>
    <section class="about"></section>
    <section class="whoiam"></section>
    <section class="goal"></section>
</body>
```

Это лучше вынести в style.css как background
```
<img src=".\icon\IMG_3136.PNG" class="mainphoto" alt="qqq">
```

В первой секции написал новые блоки. В оригинале сайта в каждом классе стоит __position: absolute__ и жестко указаны размеры widht и height.
вот они и не позволяют изменять размеры как нужно тебе.

Изменения под размер устройства определяются медиа-запросом ***@media (max-width: 650px)***
в этом блоке ты переопределяешь описание стилей, поведение которых нужно изменить (можно уменьшить шрифт заголовка, парагроф и тд)
К сожалению совсем нет времени, попробуй сверстать следующий блок сам

