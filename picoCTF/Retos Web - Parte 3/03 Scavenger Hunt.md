Puntos: 50pts
# Objetivo del Nivel

There is some interesting information hidden around this site [http://mercury.picoctf.net:39491/](http://mercury.picoctf.net:39491/). Can you find it?

# Pistas del Nivel

- You should have enough hints to find the files, don't run a brute forcer.
- 
# Solución/Resultado/Flag
- La bandera esta en dos partes. ->
```html
|   |   |
|---|---|
||<!doctype html>|
||<html>|
||<head>|
||<title>Scavenger Hunt</title>|
||<link href="[https://fonts.googleapis.com/css?family=Open+Sans\|Roboto](https://fonts.googleapis.com/css?family=Open+Sans\|Roboto)" rel="stylesheet">|
||<link rel="stylesheet" type="text/css" href="[mycss.css](http://mercury.picoctf.net:39491/mycss.css)">|
||<script type="application/javascript" src="[myjs.js](http://mercury.picoctf.net:39491/myjs.js)"></script>|
||</head>|
|||
||<body>|
||<div class="container">|
||<header>|
||<h1>Just some boring HTML</h1>|
||</header>|
|||
||<button class="tablink" onclick="openTab('tabintro', this, '#222')" id="defaultOpen">How</button>|
||<button class="tablink" onclick="openTab('tababout', this, '#222')">What</button>|
|||
||<div id="tabintro" class="tabcontent">|
||<h3>How</h3>|
||<p>How do you like my website?</p>|
||</div>|
|||
||<div id="tababout" class="tabcontent">|
||<h3>What</h3>|
||<p>I used these to make this site: <br/>|
||HTML <br/>|
||CSS <br/>|
||JS (JavaScript)|
||</p>|
||<!-- Here's the first part of the flag: picoCTF{t -->|
||</div>|
|||
||</div>|
|||
||</body>|
||</html>|
|||
```

```html
```

picoCTF{3v3ry1_l0v3s_c00k135_064663be}
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/161?assigned=1&page=1&solved=1