Puntos: 100pts
# Objetivo del Nivel

Can you find the robots? `https://jupiter.challenges.picoctf.org/problem/60915/` ([link](https://jupiter.challenges.picoctf.org/problem/60915/)) or http://jupiter.challenges.picoctf.org:60915
# Pistas del Nivel
- What part of the website could tell you where the creator doesn't want you to look?
# Solución/Resultado/Flag

```html
view-source:https://jupiter.challenges.picoctf.org/problem/60915/robots.txt
view-source:https://jupiter.challenges.picoctf.org/problem/60915/8028f.html


<!doctype html>
<html>
  <head>
    <title>Where are the robots</title>
    <link href="https://fonts.googleapis.com/css?family=Monoton|Roboto" rel="stylesheet">
    <link rel="stylesheet" type="text/css" href="style.css">
  </head>
  <body>
    <div class="container">
      
      <div class="content">
	<p>Guess you found the robots<br />
	  <flag>picoCTF{ca1cu1at1ng_Mach1n3s_8028f}</flag></p>
      </div>
      <footer></footer>
  </body>
</html>


picoCTF{ca1cu1at1ng_Mach1n3s_8028f}
```

picoCTF{ca1cu1at1ng_Mach1n3s_8028f}
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/4