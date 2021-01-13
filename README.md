<!doctype html>
<html lang="en">

<head>
    <meta charset="utf-8" />
    <link rel="stylesheet" type="text/css" href="style.css">
    <title> Лабораторная работа №4 </title>
</head>

<body>
    <header>
        <h1><strong>
                <center>Лабораторная работа №4</center>
            </strong>
        </h1>
    </header>
    <h2>navigator:</h2>
    <div id="navig" class="alert alert-waring"></div>
    <script>
        var navigate = "";
        for (var property in navigator) {
            navig += "<strong>" + property + "</strong>: " + navigator[property];
            navig += "<br />";
        }
        document.getElementById("navig").innerHTML = navig;
    </script>
        <h2>document:</h2>
    <div id="document" class="alert alert-waring"></div>
    <script>
        var document = "";
        for (var property in document) {
            document += "<strong>" + property + "</strong>: " + document[property];
            document += "<br />";
        }
        document.getElementById("document").innerHTML = document;
    </script>
        <h2>location:</h2>
    <div id="propertiesLocation" class="alert alert-warning"></div>
    <script>
        var stringPropertiesLocation = "";
        for (var property in location) {
            stringPropertiesLocation += "<strong>Свойство и метод: " + property + "</strong>";
            stringPropertiesLocation += "<p> Значение: <strong>" + location[property] + "</strong>";
            stringPropertiesLocation += "<p>Тип: <strong>" + typeof location[property] + "</strong>";
            stringPropertiesLocation += "<br><br>";
        }
        document.getElementById("propertiesLocation").innerHTML = stringPropertiesLocation;
    </script>
    <h2>window:</h2>
    <script>
        var Window;
        function WindowOpen() {
            Window = window.open("", "", "width=500,height=500");
        }
        function WindowFocus() {
            Window.focus();
        }
        function myWindowBlur() {
            Window.blur();
        }
    </script>
    <button onclick="WindowOpen()">Открыть окно</button>
    <button onclick="WindowFocus()">Развернуть окно</button>
    <button onclick="WindowBlur()">Свернуть окно</button>    
    <h2>
    </h2>
</html>
