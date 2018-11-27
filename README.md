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

- Explica el modelo de caja de CSS (margin, border y padding)
- Explica que son los selectores de CSS y pon ejemplos
- Di a quien afectan:

    p a { color: red;

    p > a { color: red; }

    h1 + h2 { color: red }

    a[class] { color: blue; }

    a[class="externo"] { color: blue; }

    a[href="http://www.ejemplo.com"] { color: blue; }
