Puntos: 100pts
# Objetivo del Nivel

Can you get the flag?
Go to this [website](http://saturn.picoctf.net:56488/) and see what you can discover.
# Pistas del Nivel
- What is the web inspector in web browsers?
# Solución/Resultado/Flag

```bash
Se utilizo una funcion del navegador para obtener el codigo html de la pagina, el comando el "CTRL + U"
view-source:saturn.picoctf.net:56488

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>On Histiaeus</title>
  </head>
  <body>
    <h1>On Histiaeus</h1>
    <p>However, according to Herodotus, Histiaeus was unhappy having to stay in
       Susa, and made plans to return to his position as King of Miletus by 
       instigating a revolt in Ionia. In 499 BC, he shaved the head of his 
       most trusted slave, tattooed a message on his head, and then waited for 
       his hair to grow back. The slave was then sent to Aristagoras, who was 
       instructed to shave the slave's head again and read the message, which 
       told him to revolt against the Persians.</p>
    <br>
    <p> Source: Wikipedia on Histiaeus </p>
	<!--picoCTF{1n5p3t0r_0f_h7ml_1fd8425b}-->
  </body>
</html>

```

picoCTF{1n5p3t0r_0f_h7ml_1fd8425b}
# Notas Adicionales

Tags:

AUTHOR:
# Referencias

https://play.picoctf.org/practice/challenge/