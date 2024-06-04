<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body style="font-family: 'Times New Roman', Times, serif;">
    <p align = "center" style="font-size: 14;">
        МИНИСТЕРСТВО НАУКИ И ВЫСШЕГО ОБРАЗОВАНИЯ <br>
        РОССИЙСКОЙ ФЕДЕРАЦИИ<br>
        ФЕДЕРАЛЬНОЕ ГОСУДАРСТВЕННОЕ БЮДЖЕТНОЕ<br>
        ОБРАЗОВАТЕЛЬНОЕ УЧРЕЖДЕНИЕ ВЫСШЕГО ОБРАЗОВАНИЯ<br>
        «САХАЛИНСКИЙ ГОСУДАРСТВЕННЫЙ УНИВЕРСИТЕТ»<br>
    </p>
    <br><br><br><br><br><br>
    <body font-size = "12">
        <p align = "center"> 
            Институт естественных наук и техносферной безопасности<br>
            Кафедра информатики<br>
            Бахтина Елена Владимировна<br>
        </p>
        <br><br><br>
        <p align = "center">
            <strong>Лабораторная работа №6. CSS»</strong><br>
            01.03.02 Прикладная математика и информатика
        </p>
        <br><br><br><br><br><br><br><br><br><br><br><br>
        <p align = "right"> 
            Научный руководитель<br>
            Соболев Евгений Игоревич
        </p>
        <br><br><br>
        <p align = "center">г. Южно-Сахалинск<br>2024 г.</p>
    </body>
    <body style="font-family: 'Times New Roman', Times, serif;">
        <h2 align = "center">Введение</h2>
        <p font-size = "12">
            <b>CSS</b> — формальный язык декодирования и описания внешнего вида документа, написанного с использованием языка разметки.
        </p>
        <br>
        <h2 align = "center">Цель и задачи</h2>
        <p align = "left" font-size = "12"> 
            Цель: решить задачи при помощи CSS.<br>
            Задачи:<br>
                1.	Придумайте селектор, который выберет абзацы <!--<p>--> внутри дивов <!--<div>-->.<br>
                2.	Придумайте селектор, который выберет все <!--<h2>--> внутри дивов <!--<div>-->.<br>
                3.	Придумайте селектор, который выберет все абзацы <!--<p>--> из элемента с id=test.<br>
                4.	Придумайте селектор, который выберет все <!--<h2>--> из элемента с id=test.<br>
                5.	Выберите все элементы с классом bbb.<br>
                6.	Выберите все элементы с классом bbb из элемента с id=test.<br>
                7.	Выберите все абзацы <!--<p>--> с классом bbb.<br>
                8.	Выберите все <!--<h2>--> с классом bbb.<br>
                9.	Выберите все абзацы <!--<p>--> с классом bbb из элемента с id=test.<br>
                10.	Выберите все элементы с классом bbb и элементы с классом xxx одновременно.<br>
                11.	Выберите все абзацы <!--<p>--> с классом bbb и <!--<h2>--> с классом xxx одновременно.<br>
                12.	Выберите все абзацы <!--<p>--> с классом bbb из id=test и все абзацы <!--<p>--> с классом xxx из id=test одновременно.<br>
                13.	Выберите все элементы из класса fff.<br>
                14.	Выберите все абзацы <!--<p>--> из класса fff.<br>
                15.	Выберите все абзацы <!--<p>--> с классом fff.<br>
                16.	Выберите все элементы с классом bbb из класса fff.<br>
                17.	Выберите все <!--<h2>--> с классом bbb из класса fff.<br>
                18.	Сделайте селектор, который выберет все ссылки из id=test, с состояния link и visited сделайте неподчеркнутыми и красными, а состояние hover - подчеркнутым и голубым.<br>
                19.	 Сделайте селектор, который выберет все ссылки с классом www, состояния link и visited сделайте подчеркнутыми и голубыми, а состояние hover - неподчеркнутым.<br>
                20.	 Сделайте селектор, который выберет все ссылки из id=test с классом www. Цвета состояний выберите самостоятельно.<br>
                21.	 Сделайте селектор, который выберет все ссылки из class=eee с классом www. Цвета состояний выберите самостоятельно.<br>
                22.	Повторите страницу по данному по образцу<br>
                23.	Повторите страницу по данному по образцу<br>
                24.	Повторите страницу по данному по образцу<br>
                25.	Повторите страницу по данному по образцу<br>
                26.	Повторите страницу по данному по образцу<br>
                27.	Повторите страницу по данному по образцу<br>
                https://www.codewars.com/kata/555de49a04b7d1c13c00000e<br>
                https://www.codewars.com/kata/588453ea56daa4af920000ca<br>
                https://www.codewars.com/kata/55e9529cbdc3b29d8c000016<br>
                https://www.codewars.com/kata/55968ab32cf633c3f8000008<br>
                https://www.codewars.com/kata/55ee3ebff71e82a30000006a<br>
                https://www.codewars.com/kata/5412509bd436bd33920011bc<br>
        </p>
        <h2 align = "center">Решение</h2>
        <p font-size = "12">Для выполнения этой лабораторной работы, я пользовалась:</p>
        <p> 1.  Материалом в сети интернет</p>
        </body>
<h3 align = "center">Файл lab6.html</h3>

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>lab6</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div>
        <p>Параграф в диве</p>
        <h2>Хеадер в диве</h2>
    </div>
    <div id="test">
        <p class="bbb">Параграф</p>
        <h2 class="bbb">Хеадер</h2>
    </div>
    <p class="bbb">Параграф</p>
    <h2 class="bbb">Хеадер</h2>
    <div class="fff">
        <p>Параграф</p>
        <p class="bbb">Параграф</p>
        <h2 class="bbb">Хеадер</h2>
    </div>
    <a href="https://music.yandex.ru/album/5144556/track/39794306" id="test">ссилка</a> <br>
    <a href="https://music.yandex.ru/album/3814492/track/31469930" class="www">ссилка</a> <br>
    <a href="https://music.yandex.ru/album/87894/track/789017" class="www">ссилка</a> <br>
    <a href="https://music.yandex.ru/album/2256801/track/43282113" class="eee www">ссилка</a> <br>
    <p class="underline">Привет, мир!</p>
    <p class="line-through">Привет, мир!</p>
    <p class="overline">Привет, мир!</p>
    <div class="square"></div>
    <div class="rectangle"></div>
    <div class="square1"></div>
    <div class="circle"></div>
    <a href="https://music.yandex.ru/album/9458494/track/60921258" class="green-link">ссылка</a><br>
    <a href="https://music.yandex.ru/album/4674671/track/37002329" class="red-link">ссылка</a><br>
    <a href="https://music.yandex.ru/album/4805573/track/37831554" class="black-link">ссылка</a>
</body>
</html>
```
<h3 align = "center">Файл style.css</h3>

```
div > p {
    color: blue;
}
div h2 {
    color: green;
}
#test p {
    font-weight: bold;
}
#test h2 {
    font-style: italic;
}
.bbb {
    background-color: lightgray;
}
#test .bbb {
    text-decoration: underline;
}
.fff {
    border: 2px solid red;
}
#test a:link, #test a:visited {
    text-decoration: none;
    color: red;
}
#test a:hover {
    text-decoration: underline;
    color: blue;
}
a.www:link, a.www:visited {
    text-decoration: underline;
    color: blue;
}
a.www:hover {
    text-decoration: none;
}
#test a.www {
    color: purple;
}
.eee a.www {
    font-style: italic;
    font-weight: bold;
}
.underline{
    text-decoration: underline;
}
.line-through{
    text-decoration: line-through;
}
.overline{
    text-decoration: overline;
}
.square{
    width: 300px;
    height: 300px;
    border: 1px solid red;
}
.rectangle{
    margin-top: 5px;
    width: 500px;
    height: 200px;
    border: 1px dashed blue;
}
.square1{
    margin-top: 5px;
    width: 300px;
    height: 300px;
    border: 1px dashed green;
    border-radius: 5% 12% 5% 12%;
}
.circle{
    margin-top: 5px;
    width: 100px;
    height: 100px;
    border: 1px solid red;
    border-radius: 50%;
}
.green-link{
    color: green;
    text-decoration: underline;
}
.red-link{
    color: red;
    text-decoration: underline;
}
.black-link{
    color: black;
    text-decoration: none;
}
```
</html>
<br>
 <h2 align = "center">Вывод</h2>
 <p align = "left" font-size = "12">
    По итогу данной лабороторной работы, я научилась новым интересным вещам в CSS 😊   
</p>
</body>
</html>