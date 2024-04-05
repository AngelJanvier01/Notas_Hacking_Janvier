Puntos: 100pts
# Objetivo del Nivel

Can you get the flag?Go to this [website](http://saturn.picoctf.net:61941/) and see what you can discover.
# Pistas del Nivel
- Is there more code than what the inspector initially shows?
# Solución/Resultado/Flag

```bash
Se utilizo el inspector del navegador, la bandera se divide en dos partes,
```

```js
script.js parte 1:

function greetings()
{
  alert("This code is in a separate file!");
}

//  f7w_2of2_6edef411}
```

```css
style.css parte 2: 

body {
  background-color: lightblue;
}

/*  picoCTF{1nclu51v17y_1of2_  */

```

picoCTF{1nclu51v17y_1of2_f7w_2of2_6edef411}
# Notas Adicionales

Tags:

AUTHOR:
# Referencias

https://play.picoctf.org/practice/challenge/