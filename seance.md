# P5*js

Es una librería de JavaScript que tiene el mismo objetivo que Processing, hacer el código informático accesible a diseñadores, artistas, educadores y presonas que quieren introducirse en el mundo de la programación.

## Estructura Básica

Un script de p5 se compone de tres funciones esenciales:

**setup:** Contiene los elementos estáticos y diferentes parámetro de configuración inicial, es obligatorio su uso.

´´´JavaScript
	function setup(){

	};
´´´

**draw:** Es la función que contiene los diferentes elementos que se visualizan en pantalla y los cuales puede ser dinámicos e interactivos, aunque su uso no es obligatorio esta función es casi omnipresente en las diferentes creaciones.

´´´JavaScript
	function draw(){

	};
´´´

**oreload:** Permite cargar el contenido el contenido antes de empezar la ejecución de setup() y draw()

´´´JavaScript
	function preload(){

	};
´´´


## Figuras Geométricas Básicas y Texto

La mayoria de figuras tienen en común dos propiedades básicas posición en X y posición en y, las otras propiedades varían según figura.

´´´JavaScript
	point(corX, corY, corZ)
	ellipse(corX, corY, ancho, alto )
	rec(corX, corY, ancho, alto, curva_de_las_esquinas)
´´´
Otras figuras como triángulos  y cuadriláteros hay que darle la coordenada de cada punto o intercepción de la figura.

´´´JavaScript
	line(px1, py1, px2, py2)
	triangle(px1, py1, px2, py2, px3, py3)
	quad(px1, py1, px2, py2, px3, py3, px4, py4)
´´´

## Algunos Atributos

### Generales

* **width** y **height hace referencia al ancho y alto del canvas con el que se trabaja

* **displayWidth** y **displayHeight** para saber ancho y alto de la pantalla 

* **windowWidth*** y **windowHeight** para ancho y alto dela ventana


### Para el setup

* **frameRate(x)** x representa el número de fotos por segundo que proyectará la función draw por segundo.

* **noCursor()** Desaparece el puntero del area de la función draw()

* **noLoop()** Para las fotos por segundo en draw()

* **background()** Da el color al fondo del area de trabajo, esta también se puede usar en la función draw()

	
### Para los objetos

* **fill(x)** Establece el color del relleno del objeto

* **stroke()** Establece el color del borde dela Figuras

* **strokeWeight()** define el ancho del borde

* **noFill()**, **noStroke()**, quitan el relleno y el borde de la Figuras


