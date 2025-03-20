# Pokerjs
Small frontend project using js,html, and css

# Representación de Cartas Francesas

Crea un tipo de objetos que sirva para representar **Cartas francesas**. Estos objetos tendrán dos propiedades:

- **palo**: Un carácter (c, d, p, t)
- **valor**: Un número del 1 al 13

Los objetos de este tipo se construyen indicando el palo y el valor. Si hay fallos en los datos, se devuelve un objeto `Carta` con valores `null` en palo y valor.

## Métodos de las Cartas

Las cartas tendrán estos métodos:

- **darValor**: Que recibe un palo y un valor para, con ellos, modificar la carta. Ante datos incorrectos, no cambia nada en la carta.
- **toString**: Método para devolver en forma de texto entendible el valor de la carta. Por ejemplo: "As de Picas".

## Objeto Baraja

Además, habrá otro tipo de objeto: **Baraja**. La idea es que represente una baraja de cartas francesas. Tendrá los siguientes detalles:

- La baraja la forman 52 cartas. Para ello tendrá la propiedad `cartas` que será un array de 52 cartas. Al construir la Baraja se rellenan las cartas en el siguiente orden: por palos y cada palo con las cartas del 1 al 13. No se podrá acceder directamente al array fuera del objeto.
- El método **barajar** permite barajar las cartas, es decir, desordenarlas de forma aleatoria.
- El método **toString** permite obtener la baraja en forma de texto para saber qué cartas hay en la baraja y cómo están ordenadas.
- El método **reparteCarta** devuelve la última carta de la Baraja, desapareciendo dicha carta del array de cartas.

## Objeto Jugador

Otro tipo de objeto necesario será **Jugador**.

- El Jugador tendrá una propiedad `mano` que almacenará las cartas que le repartan.
- Un método **nuevaCarta** que se encargará de ir añadiendo cartas al Jugador (hasta 5 cartas para jugar al póker).
- Un método **toString** permite obtener las cartas en la mano en forma de texto para saber qué cartas tiene el jugador.
- Además, necesitará un método que indique la jugada de póker que tiene en la mano (Pareja, Doble pareja, Trío, Escalera, Color, Full, Póker o Escalera de color).

## Página Web

Crea una página web que, utilizando JavaScript, cree una baraja de cartas, barajee y reparta cinco cartas a un jugador.

La página deberá mostrar la imagen de estas cinco cartas por pantalla (utilizar los ficheros SVG que encontrarás en el directorio `cartas`) e indicar la jugada obtenida por el jugador.
