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

ASCII es un código en el cuál se representa cada carácter con un byte, en ASCII es posible representar 128 carácteres. Unicode es un código que asigna un número a cada carácter, tiene capacidad de codificar 1.1 millones de carácteres, es la codificación mas utilizada en la actualidad.

Muchos protocolos de bajo nivel solo soportan ASCII, esto limita también lo que puedan hacer las aplicaciones de red que emplean dichos protocolos. Para resolver este problema se creó el mecanismo **IDNA** (Internationalizing Domain Names in Applications) el cual define una manera de interpretar caracteres no-ASCII para que las aplicaciones de red puedan interactuar con las capas inferiores y quizás tambien permitir al usuario interactuar con su encoding favorito.
Los navegadores mas modernos utilizan **IDNA** para decodificar dominios en unicode, permitiendonos entrar a links que no esten codificados en ASCII.

### Referencias

https://nedbatchelder.com/text/unipain.html

https://en.wikipedia.org/wiki/Domain_Name_System

https://en.wikipedia.org/wiki/Internationalized_domain_name

---

**[README](README.md)**
