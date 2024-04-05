Puntos: 100pts
# Objetivo del Nivel

Can you get the flag?
Go to this [website](http://saturn.picoctf.net:49386/) and see what you can discover.
# Pistas del Nivel
- How is the password checked on this website?
# Solución/Resultado/Flag

```bash
Nos pidio ingresar constraseña y usuario pero como no lo conozco, me dio por inspeccionar y salio un archivo llamado "secure.js"
que dice:

function checkPassword(username, password)
{
  if( username === 'admin' && password === 'strongPassword098765' )
  {
    return true;
  }
  else
  {
    return false;
  }
}

asi que seria logico ingresar esos datos de acceso :)

http://saturn.picoctf.net:49386/admin.php

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <link rel="stylesheet" href="style.css">
    <title>Secure Customer Portal</title>
  </head>
  <body>
    ==="picoCTF{j5_15_7r4n5p4r3n7_b0c2c9cb}"===  </body>
</html>

```

picoCTF{j5_15_7r4n5p4r3n7_b0c2c9cb}
# Notas Adicionales

Tags:

AUTHOR:
# Referencias

https://play.picoctf.org/practice/challenge/