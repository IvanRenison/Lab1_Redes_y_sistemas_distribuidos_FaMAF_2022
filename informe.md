# Informe lab 1

- Fuentes, Tiffany
- Renison, Iván
- Schachner, Álvaro

---

**[README](README.md)**

---

# Contenido

- [Informe lab 1](#informe-lab-1)
- [Contenido](#contenido)
- [Punto estrella](#punto-estrella)
  - [Encoding](#encoding)
- [Referencias](#referencias)

# Punto estrella

## Encoding

ASCII es un código en el cuál se representa cada carácter con un byte, en ASCII es posible representar 256 carácteres. Unicode es un código que asigna un número a cada carácter, tiene capacidad de codificar 1.1 millones de carácteres, es la codificación mas utilizada en la actualidad.

En Python 2 tenemos objetos **"str"** que guarda texto plano como un stream de bytes (ASCII), y los objetos **"unicode"** los cuales guardan código Unicode, estos últimos se indican utilizando `u""`, y colocando el mensaje dentro de las comillas, y usando `\u` se puede insertar cualquier código Unicode. En Python 2 la función Encode() se utiliza para convertir un objeto unicode a un stream de bytes, y la función Decode() para convertir un string de bytes a un objeto Unicode.

Con la actualización a Python 3 se decidio manejar los strings con codificación Unicode, lo cual quiere decir Encode() se utiliza para convertir cualquier string a un stream de bytes.

## DNS

DNS es el protocolo para obtener la dirección IP a partir de un dominio (como por ejemplo, [example.com](http://example.com/)). Este protocolo solo acepta strings de caracteres ASCII para los dominios, por lo cuál, para los dominios no ASCII (como [ñandú.com](http://ñandú.com/)) el string del dominio se tiene que codificar a ASCII.

En el código, la obtención de la dirección ip se hace llamando a la función `socket.gethostbyname`. Está función aplica la codificación automáticamente, por lo que no es necesario hacer nada especial para que funcionen los dominios no ASCII.

### Referencias

https://nedbatchelder.com/text/unipain.html

---

**[README](README.md)**