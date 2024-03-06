Puntos: 40pts
# Objetivo del Nivel

Who doesn't love cookies? Try to figure out the best one. [http://mercury.picoctf.net:27177/](http://mercury.picoctf.net:27177/)

# Pistas del Nivel

- none
# Solución/Resultado/Flag

```bash
hay que jugar con el valor de las cookies, le puse valores superiores para descartar rangos superiores,
llegue a que 30 era el maximo asi que jugue con el valor hasta que llegue a +18
```

```html
|   |   |
|---|---|
||<!DOCTYPE html>|
||<html lang="en">|
|||
||<head>|
||<title>Cookies</title>|
|||
|||
||<link href="[https://maxcdn.bootstrapcdn.com/bootstrap/3.2.0/css/bootstrap.min.css](https://maxcdn.bootstrapcdn.com/bootstrap/3.2.0/css/bootstrap.min.css)" rel="stylesheet">|
|||
||<link href="[https://getbootstrap.com/docs/3.3/examples/jumbotron-narrow/jumbotron-narrow.css](https://getbootstrap.com/docs/3.3/examples/jumbotron-narrow/jumbotron-narrow.css)" rel="stylesheet">|
|||
||<script src="[https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js](https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js)"></script>|
|||
||<script src="[https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js](https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js)"></script>|
|||
||</head>|
|||
||<body>|
|||
||<div class="container">|
||<div class="header">|
||<nav>|
||<ul class="nav nav-pills pull-right">|
||<li role="presentation"><a href="[/reset](http://mercury.picoctf.net:27177/reset)" class="btn btn-link pull-right">Home</a>|
||</li>|
||</ul>|
||</nav>|
||<h3 class="text-muted">Cookies</h3>|
||</div>|
|||
||<div class="jumbotron">|
||<p class="lead"></p>|
||<p style="text-align:center; font-size:30px;"><b>Flag</b>: <code>picoCTF{3v3ry1_l0v3s_c00k135_064663be}</code></p>|
||</div>|
|||
|||
||<footer class="footer">|
||<p>&copy; PicoCTF</p>|
||</footer>|
|||
||</div>|
||</body>|
|||
||</html>|
```

picoCTF{3v3ry1_l0v3s_c00k135_064663be}
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/132