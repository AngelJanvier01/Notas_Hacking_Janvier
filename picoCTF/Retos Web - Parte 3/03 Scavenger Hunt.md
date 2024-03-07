Puntos: 50pts
# Objetivo del Nivel

There is some interesting information hidden around this site [http://mercury.picoctf.net:39491/](http://mercury.picoctf.net:39491/). Can you find it?

# Pistas del Nivel

- You should have enough hints to find the files, don't run a brute forcer.
- 
# Solución/Resultado/Flag
- La bandera esta en dos partes. ->
- Definitivamente estaba en tres partes. ->
- nonono eran mas jajaja son 5 partes ->
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

```css
div.container {
    width: 100%;
}

header {
    background-color: black;
    padding: 1em;
    color: white;
    clear: left;
    text-align: center;
}

body {
    font-family: Roboto;
}

h1 {
    color: white;
}

p {
    font-family: "Open Sans";
}

.tablink {
    background-color: #555;
    color: white;
    float: left;
    border: none;
    outline: none;
    cursor: pointer;
    padding: 14px 16px;
    font-size: 17px;
    width: 50%;
}

.tablink:hover {
    background-color: #777;
}

.tabcontent {
    color: #111;
    display: none;
    padding: 50px;
    text-align: center;
}

#tabintro { background-color: #ccc; }
#tababout { background-color: #ccc; }

/* CSS makes the page look nice, and yes, it also has part of the flag. Here's part 2: h4ts_4_l0 */
```

```js
La segunda parte la encontre haciendo una busqueda en la web, por la pista que nos dan en el archivo my.js

function openTab(tabName,elmnt,color) {
    var i, tabcontent, tablinks;
    tabcontent = document.getElementsByClassName("tabcontent");
    for (i = 0; i < tabcontent.length; i++) {
	tabcontent[i].style.display = "none";
    }
    tablinks = document.getElementsByClassName("tablink");
    for (i = 0; i < tablinks.length; i++) {
	tablinks[i].style.backgroundColor = "";
    }
    document.getElementById(tabName).style.display = "block";
    if(elmnt.style != null) {
	elmnt.style.backgroundColor = color;
    }
}

window.onload = function() {
    openTab('tabintro', this, '#222');
}

/* How can I keep Google from indexing my website? */

Asi que basto con hacer una busqueda con el comando aprendido en la clase: **site:domain.com/robots.txt**
```

```html
|   |   |
|---|---|
||User-agent: *|
||Disallow: /index.html|
||# Part 3: t_0f_pl4c|
||# I think this is an apache server... can you Access the next flag?|
```

```html

site:mercury.picoctf.net:39491/.htaccess

# Part 4: 3s_2_lO0k
# I love making websites on my Mac, I can Store a lot of information there.
```

```html
.DS_Store


Congrats! You completed the scavenger hunt. Part 5: _f7ce8828}

```

picoCTF{th4ts_4_l0t_0f_pl4c3s_2_lO0k_f7ce8828}
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/161?assigned=1&page=1&solved=1