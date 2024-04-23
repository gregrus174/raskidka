<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>bestsite</title>
    <style>
        @font-face {
    font-family: 'SHRIFT'; /* semen huesoska */
    src: url('SHRIFT.ttf') format('truetype'); /* Путь к файлу шрифта относительно текущей директории */
}
        body {
            background-image: url('black-watercolor-background.jpg'); /* Устанавливаем фоновое изображение */
            background-size: 1600px 750px; /* Устанавливаем размер фонового изображения */
            color: white; /* Устанавливаем цвет текста */
            font-family: SHRIFT; /* Устанавливаем шрифт */
            text-align: left; /* Выравниваем текст по левому краю */
            padding-top: -30px; /* Устанавливаем отступ сверху */
            padding-left: 30px; /* Устанавливаем отступ слева */
        }
        h1 {
            text-shadow: /* Добавляем тень тексту */
            -1px -1px 0 #48D1CC,  
            1px -1px 0 #48D1CC,
            -1px 1px 0 #48D1CC,
            1px 1px 0 #48D1CC;
            font-size: 50px; /* Устанавливаем размер шрифта */
            text-transform: uppercase; /* Преобразуем текст в верхний регистр */
        }
        button {
            color: white; /* Устанавливаем цвет текста */
            padding: 20px 30px; /* Устанавливаем внутренние отступы */
            border: none; /* Убираем границу */
            cursor: pointer; /* Устанавливаем курсор при наведении на кнопку */
            text-transform: uppercase; /* Преобразуем текст в верхний регистр */
            font-family: SHRIFT, sans-serif; /* Устанавливаем шрифт */
            font-size: 20px; /* Устанавливаем размер шрифта */
            display: block; /* Блочное отображение */
            margin-bottom: 25px; /* Устанавливаем отступ снизу */
            transition: background-color 0.5s; /* Устанавливаем плавный переход цвета фона при наведении курсора */
        }
        button:hover {
            background-color: #555; /* Устанавливаем цвет фона при наведении курсора */
            transform: scale(1.01); /* Увеличиваем размер кнопки при наведении курсора */
        }
        .Ascent {
            background-color: #B0E0E6; /* Устанавливаем цвет фона кнопки */
            width: 150px; /* Устанавливаем ширину кнопки */
            position: relative; /* Позиционируем элемент относительно его обычного положения */
        }
        .Bind {
            background-color: #D3D3D3; /* Устанавливаем цвет фона кнопки */
            width: 150px; /* Устанавливаем ширину кнопки */
            position: relative; /* Позиционируем элемент относительно его обычного положения */
        }
        .Lotus {
            background-color: #A9A9A9; /* Устанавливаем цвет фона кнопки */
            width: 150px; /* Устанавливаем ширину кнопки */
            position: relative; /* Позиционируем элемент относительно его обычного положения */
        }
        .Breeze {
            background-color: #778899; /* Устанавливаем цвет фона кнопки */
            width: 150px; /* Устанавливаем ширину кнопки */
            position: relative; /* Позиционируем элемент относительно его обычного положения */
        }
        .Icebox {
            background-color: #5F9EA0; /* Устанавливаем цвет фона кнопки */
            width: 150px; /* Устанавливаем ширину кнопки */
            position: relative; /* Позиционируем элемент относительно его обычного положения */
        }
        .Sunset {
            background-color: #2F4F4F; /* Устанавливаем цвет фона кнопки */
            width: 150px; /* Устанавливаем ширину кнопки */
            position: relative; /* Позиционируем элемент относительно его обычного положения */
        }
        .slideshow-container {
            max-width:500px; /* Устанавливаем максимальную ширину контейнера */
            position: relative; /* Позиционируем элемент относительно его обычного положения */
            margin-right: 200px; /* Устанавливаем отступ справа */
            float: right; /* Обтекание элементов справа */
            font-family: Arial;
        }

        .text {
            color: #ffffff; /* Устанавливаем цвет текста */
            font-size: 40px; /* Устанавливаем размер шрифта */
            padding: 8px 12px; /* Устанавливаем внутренние отступы */
            position: absolute; /* Позиционируем элемент относительно его первого родителя с позиционированием, кроме static */
            bottom: 8px; /* Устанавливаем отступ снизу */
            width: 100%; /* Устанавливаем ширину */
            text-align: center; /* Выравниваем текст по центру */
        }

        .numbertext {
            color: #ffffff; /* Устанавливаем цвет текста */
            font-size: 20px; /* Устанавливаем размер шрифта */
            padding: 8px 12px; /* Устанавливаем внутренние отступы */
            position: absolute; /* Позиционируем элемент относительно его первого родителя с позиционированием, кроме static */
            top: 0; /* Устанавливаем отступ сверху */
        }

        .fade {
            -webkit-animation-name: fade; /* Имя анимации для браузеров, использующих вендорные префиксы */
            -webkit-animation-duration: 10s; /* Продолжительность анимации */
            animation-name: fade; /* Имя анимации */
            animation-duration: 2s; /* Продолжительность анимации */
        }
        @-webkit-keyframes fade {
            from {opacity: .4} /* Начальное значение прозрачности */
            to {opacity: 1} /* Конечное значение прозрачности */
        }
        @keyframes fade {
            from {opacity: .4} /* Начальное значение прозрачности */
            to {opacity: 1} /* Конечное значение прозрачности */
        }

        @media only screen and (max-width: 300px) {
            .prev, .next,.text {font-size: 11px} /* Устанавливаем размер шрифта для элементов .prev, .next и .text */
        }

        .dropdown {
          position: relative; /* Позиционируем элемент относительно его первого родителя с позиционированием, кроме static */
          display: inline-block; /* Отображаем элемент как строчно-блочный с возможностью установки ширины и высоты */
        }

        .dropdown-content {
          display: none; /* Скрываем содержимое элемента */
          position: absolute; /* Позиционируем элемент относительно ближайшего позиционированного предка */
          background-color: #90EE90; /* Устанавливаем цвет фона */
          min-width: 160px; /* Устанавливаем минимальную ширину */
          box-shadow: 0px 0px 50px -20px #32CD32;
          z-index: 1; /* Устанавливаем порядок наложения */
          top: 0px; /* Устанавливаем отступ сверху */
          left: 100%; /* Устанавливаем отступ слева */
        }

.dropdown-content a {
color: white; /* Устанавливаем цвет текста */
padding: 12px 30px; /* Устанавливаем внутренние отступы */
text-decoration: none; /* Убираем подчеркивание текста */
display: block; /* Отображаем элемент как блочный */
background-color: #F4A460; /* Устанавливаем цвет фона */
cursor: pointer; /* Устанавливаем курсор при наведении на элемент */
}
.dropdown-content a.dropdown-link {
color: white;
padding: 12px 30px;
text-decoration: none;
display: block;
background-color: #4682B4;
cursor: pointer;
}

.dropdown-content a.dropdown-link:hover {
background-color: rgb(50, 110, 180);
}
.dropdown-content a:hover {background-color: #FF8C00} /* Устанавливаем цвет фона при наведении на элемент */

        .Ascent:hover .dropdown-content {
          display: block; /* Отображаем содержимое при наведении на элемент */
        }

    </style>
</head>
<body>
    <h1>lineups for viper</h1>
    <div class="slideshow-container">
        <div class="mySlides fade">
            <div class="numbertext">1 / 228</div>
            <img src="Valorant Viper Cat Icon.jpg" style="width:100%">
            <div class="text">lol</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">2 / 228</div>
            <img src="cat1.jpg" style="width:100%">
            <div class="text">kek</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">3 / 228</div>
            <img src="cat2.jpg" style="width:100%">
            <div class="text">sperm</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">4 / 228</div>
            <img src="(1).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">5 / 228</div>
            <img src="(2).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">6 / 228</div>
            <img src="(3).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">7 / 228</div>
            <img src="(4).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">8 / 228</div>
            <img src="(5).jpg" style="width:100%">
            <div class="text">sperm</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">9 / 228</div>
            <img src="(6).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">10 / 228</div>
            <img src="(7).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">11 / 228</div>
            <img src="(8).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">12 / 228</div>
            <img src="(9).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">13 / 228</div>
            <img src="(10).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">14 / 228</div>
            <img src="(11).jpg" style="width:100%">
            <div class="text">sperm</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">15 / 228</div>
            <img src="(12).jpg" style="width:100%">
            <div class="text">sperm</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">16 / 228</div>
            <img src="(13).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">17 / 228</div>
            <img src="(14).jpg" style="width:100%">
            <div class="text">sperm</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">18 / 228</div>
            <img src="(15).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">19 / 228</div>
            <img src="(16).jpg" style="width:100%">
            <div class="text">sperm</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">20 / 228</div>
            <img src="(17).jpg" style="width:100%">
            <div class="text">sperm</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">21 / 228</div>
            <img src="(18).jpg" style="width:100%">
            <div class="text">sperm!</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">22 / 228</div>
            <img src="(19).jpg" style="width:100%">
            <div class="text">sperm</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">23 / 228</div>
            <img src="(20).jpg" style="width:100%">
            <div class="text">sperm</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">24 / 228</div>
            <img src="(21).jpg" style="width:100%">
            <div class="text">sperm</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">25 / 228</div>
            <img src="(22).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">26 / 228</div>
            <img src="(23).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">27 / 228</div>
            <img src="(24).jpg" style="width:100%">
            <div class="text">sperm</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">28 / 228</div>
            <img src="(25).jpg" style="width:100%">
            <div class="text">sperm</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">29 / 228</div>
            <img src="(26).jpg" style="width:100%">
            <div class="text">sperm</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">30 / 228</div>
            <img src="(27).jpg" style="width:100%">
            <div class="text">sperm</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">31 / 228</div>
            <img src="(28).jpg" style="width:100%">
            <div class="text">sperm</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">32 / 228</div>
            <img src="(29).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">33 / 228</div>
            <img src="(30).jpg" style="width:100%">
            <div class="text">sperm</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">34 / 228</div>
            <img src="(32).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">35 / 228</div>
            <img src="(33).jpg" style="width:100%">
            <div class="text">sperm</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">36 / 228</div>
            <img src="(34).jpg" style="width:100%">
            <div class="text">sperm</div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">37 / 228</div>
            <img src="(35).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">38 / 228</div>
            <img src="(36).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">39 / 228</div>
            <img src="(37).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">40 / 228</div>
            <img src="(38).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">41 / 228</div>
            <img src="(39).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">42 / 228</div>
            <img src="(40).jpg" style="width:100%">
            <div class="text"></div>
        </div>
        <div class="mySlides fade">
            <div class="numbertext">43 / 228</div>
            <img src="(41).jpg" style="width:100%">
            <div class="text"></div>
        </div>
    </div>

<div class="Ascent">
  <button class="Ascent">Ascent</button>
  <div class="dropdown-content">
    <a href="ascent_t_side.html"><strong>T side</strong></a>
    <a href="ascent_ct_side.html" class="dropdown-link"><strong>CT side</strong></a>
  </div>
</div>

    <div class="Ascent">
      <button class="Bind">Bind</button> <!-- Создаем кнопку -->
      <div class="dropdown-content"> <!-- Создаем выпадающий контент -->
    <a href="bind_t_side.html"><strong>T side</strong></a> <!-- Ссылка на страницу с настройками Ascent для T side -->
    <a href="bind_ct_side.html" class="dropdown-link"><strong>CT side</strong></a> <!-- Ссылка на страницу с настройками Ascent для CT side -->
      </div>
    </div>

    <div class="Ascent">
      <button class="Lotus">Lotus</button> <!-- Создаем кнопку -->
      <div class="dropdown-content"> <!-- Создаем выпадающий контент -->
    <a href="lotus_t_side.html"><strong>T side</strong></a> <!-- Ссылка на страницу с настройками Ascent для T side -->
    <a href="lotus_ct_side.html" class="dropdown-link"><strong>CT side</strong></a> <!-- Ссылка на страницу с настройками Ascent для CT side -->
      </div>
    </div>

    <div class="Ascent">
      <button class="Breeze">Breeze</button> <!-- Создаем кнопку -->
      <div class="dropdown-content"> <!-- Создаем выпадающий контент -->
    <a href="breeze_t_side.html"><strong>T side</strong></a> <!-- Ссылка на страницу с настройками Ascent для T side -->
    <a href="breeze_ct_side.html" class="dropdown-link"><strong>CT side</strong></a> <!-- Ссылка на страницу с настройками Ascent для CT side -->
      </div>
    </div>

    <div class="Ascent">
      <button class="Icebox">Icebox</button> <!-- Создаем кнопку -->
      <div class="dropdown-content"> <!-- Создаем выпадающий контент -->
    <a href="icebox_t_side.html"><strong>T side</strong></a> <!-- Ссылка на страницу с настройками Ascent для T side -->
    <a href="icebox_ct_side.html" class="dropdown-link"><strong>CT side</strong></a> <!-- Ссылка на страницу с настройками Ascent для CT side -->
      </div>
    </div>

    <div class="Ascent">
      <button class="Sunset">Sunset</button> <!-- Создаем кнопку -->
      <div class="dropdown-content"> <!-- Создаем выпадающий контент -->
    <a href="sunset_t_side.html"><strong>T side</strong></a> <!-- Ссылка на страницу с настройками Ascent для T side -->
    <a href="sunset_ct_side.html" class="dropdown-link"><strong>CT side</strong></a> <!-- Ссылка на страницу с настройками Ascent для CT side -->
      </div>
    </div>

    <script>
        var slideIndex = 0;
        showSlides();
      
        function showSlides() {
            var i;
            var slides = document.getElementsByClassName("mySlides");
            for (i = 0; i < slides.length; i++) {
                slides[i].style.display = "none"; 
            }
            slideIndex++;
            if (slideIndex > slides.length) {slideIndex = 1} 
            slides[slideIndex-1].style.display = "block"; 
            setTimeout(showSlides, 3000);
        }
    </script>
</body>
</html>

