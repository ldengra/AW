# AW
ejercicios clase Aplicaciones Web

- estructura mínima de una web
```html
<!DOCTYPE html>
<html>
<head>
	<title></title>
</head>
<body>

</body>
</html>
```

- explica las 3 formas de usar CSS en HTML
```html
Interno: El interno es creando una etiqueta de style y aplicandolo en la etiqueta deseada, por ejemplo 
<style>
p {
	text-align: center
}
</style>

Externo: Creamos un archivo con extension .css con los estilos que queremos aplicar y lo instertamos en nuestro codigo de esta manera
 <head>
<link rel="style" type="text/css" href="rutaDelArchivo.css">
</head>

En linea: Se coloca el codigo en la misma linea de la etiqueta
<p style="color:red; font-size:10px;> esto es un css en linea</p>
```
- crea una lista sin ordenar con 5 ingredientes de una receta de cocina
```html
<ul>
	<li>Arroz</li>
	<li>Pollo</li>
	<li>Conejo</li>
	<li>Judia Ancha</li>
	<li>Garrofon</li>
</ul>
```
- como se puede incluir javascript en HTML
```html
Dentro del head podemos crear la estiqueta script y la opcion, en este caso que nos abra una ventana al iniciar la pagina que diga hola mundo
<script type="text/javascript">
		alert("hola mundo");
	</script>
```
- ¿Que diferencia hay entre una clase y una ID
```html
ID: El selector id tiene que ser que tener un valor unico, no tiene que haber otra id con el mismo nombre. Este selector tiene prioridad ante la clase, ya que tiene un peso mayor en el codigo. Las propiedades se aplicarian, pero la sintaxis seria incorrecta.
<div id="ID">solo hay que usarse una vez</div>

Class: Este selector puede ser utilizado en mas elementos y se aplicarian los estilos en los diferentes elementos, viene bien cuando quieres usar el mismo estilo en diferentes elementos y nos ahorramos codigo
<div class="Clase">Usando esta clase, se aplica el estilo a todas las etiquetas que identifiquemos con "Clase"</div>
```
- código para hacer un enlace a otra página y que esta se abra en una nueva ventana
```html
 <a href="https://google.es" target="_blank">Link a Google</a> 
```
- ¿Qué son las pseudoclases?, pon ejemplos.
```html
Las pseudoclases sirven para dar un estilo un elemento dependiendo de donde esten colocados en la estructura del documento. Se definen añadiendo 2 puntos antes de la clase a la que se quiere añadir el pseudoelemento. Por ejemplo con el target podemos hacer que un link cambie de color al ponerte encima.
:active :hover :target
```
- Explica el modelo de caja de CSS (margin, border y padding)
```html
Las cajas son la base del diseño web, son cajas rectagulares con sus caracteristicas como el padding, borde, margen con las que podemos modificar las medidas de las cajas y de las etiquetas. La suma de estos estilos no puede ser superior a la de la caja principal, ya que se descuadraria la pagina.
Tambien tenemos el width y el height para definir la altura y la anchura de la pagina. Tenemos la opcion de ir anidando cajas unas con otras para poder diversificar el codigo y manejarlo mejor
```
- Explica que son los selectores de CSS y pon ejemplos
```html
Existen varios tipos de selectores.
	Selector universal: Se utiliza para seleccionar todos los elementos de la pagina, con este ejemplo podemos poner un padding de 5px en todas los elementos html
		*{
			paddign: 5px;
		  }
	Selector tipo etiqueta: Selecciona solo los elementos de html que identificamos antes, por ejemplo, si queremos escoger todos los parrafos, lo hariamos asi.
		p {
			padding: 5px;
		  }
		h1{
			color: black;
		  }
	Selector descendente: Selecciona los elementos que estan anidados en otros elementos, en este ejemplo selecciona todos los elementos <span> que se encuentra dentro de un elemento <p>
		p span { 
			color: red; 
			}
Tambien existen los selectores de clase e ID.
	<p class="selectorclase">asi seleccionamos un selector de clase</p>
	<p id="selectorid">asi seleccionamos un selector id</p>
```
- Di a quien afectan:

    p a { color: red;
```html
los elementos a que esten dentro de pe se vuelven rojos
```

    p > a { color: red; }
```html
los hijos directos de p se vuelven rojos
```

    h1 + h2 { color: red }
```html
los elementos h2 se vuelven rojos si estan despues de un h1
```

    a[class] { color: blue; }
```html
tods los enlaces que esten en clases se vuelven azules
```

    a[class="externo"] { color: blue; }
```html
los enlaces con la clase externo se vuelven azules
```

    a[href="http://www.ejemplo.com"] { color: blue; }
```html
los enlaces que estan dentro se vuelven azules
```
