# AW
## Paginas Web
<b>1.-Estructura mínima de una web</b>
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
<b>2.-Explica las 3 formas de usar CSS en HTML </b><br>
La primera forma es en la misma linea<br>
-Ejemplo:
```html
	<p style="color:blue;">Ejemplo de CSS en la misma linea</p>
```
La segunda forma es en un <code><style></code> dentro del elemento <code>head</code> <br>
-Ejemplo:
```html
<!DOCTYPE html>
<html>
<head>
<style>
p    {
	color: red;}
</style>
</head>
<body>

<h1>Cabecera</h1>
<p>Un paragrafo.</p>

</body>
</html>
```
Por ultimo crear un archivo CSS y enlazarlo con el html<br>
-Ejemplo:
```html
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" href="estilos.css">
</head>
<body>

<h1>Cabecera</h1>
<p>Un paragrafo.</p>

</body>
</html>
```
<b>3.-Crea una lista sin ordenar con 5 ingredientes de una receta de cocina</b>
```html
<ul>
	<li>arina</li>
	<li>Limón</li>
	<li>Pimienta</li>
	<li>Sal</li>
	<li>Ajo</li>
</ul>
```
<b>4.-Como se puede incluir javascript en HTML</b> <br>
 Se incorpora con la etiqueta <code><script></code> y entre los parentesis colocas el id/class para que <br>
	identifique a que elemento tiene que ejecutarse.
```html
	<script>
	document.getElementById("Prueba").innerHTML = "Prueba JavaScript";
</script>
```
<b>5.-¿Que diferencia hay entre una clase y una ID </b><br><br>
	Una clase engloba varios elementos para que tengan el mismo codigo CSS, "p" y "h2" pueden tener la misma clase, <br>
	en cambio un ID solo puede haber un ID unico que pertenezca a un elemento aparte el Id diferencia entre minusculas y <br> 
	mayusculas, y no puede contener un espacio ni tabulaciones, al conterio que una clase.<br><br>
<b>6.-Código para hacer un enlace a otra página y que esta se abra en una nueva ventana</b><br>
	Hay que colocar el <code>target</code> y dentro seleccionar la opcion <code>_blank</code><br> 
	para que se habra en una nueva ventana
```html
<a href="https://www.google.com" target="_blank">Ejercicio 6</a> 
```
<b>7.-¿Qué son las pseudoclases?, pon ejemplos.</b><br><br>
Se utiliza para definir un estado a un elemento. Da estilos cuando pasamos el cursor por encima del texto, cuando el enlace<br>
ha sido visitado o cuando no han sido visitados o en una caja de texto cuando lo has seleccionado
```html
<html>
<head>
<style>
/* Cuando el link no esta visitado*/
a:link {
    color: orange;
}

/* Cuando el link esta visitado */
a:visited {
    color: purple;
}

/* Cuando pasas el raton por encima */
a:hover {
    color: red;
}

/* cuando lo seleccionas */
a:active {
    color: blue;
}

</style>
</head>
<body>

<p><a href="https://www.google.com" target="_blank">Ejercicio 7</a></p>
</body>
</html>

También puedes usarlo en DIVs o en p, por ejemplo puedes hacer que aparezca el p<br>
cuando el cursor esta encima del DIV<br>

<html>
<head>
<style>
p {
    display: none;
    background-color: red;
    padding: 20px;
    text-align:center;
    font-size:100px;
}

div:hover p {
    display: block;
}
</style>
</head>
<body>

<div>No pases el raton por encima
  <p>Warning!!!!</p>
</div>

</body>
</html>
```
Y Tambien estan la pseudo clases de primer hijo, por ejemplo, si tienes un DIV y solo al primer hijo le quieres dar<br>
un estado puedes con el comando <code>div:first-child</code> en el style del HTML
-Ejemplo:
```html
p i:first-child {
    color: white;
    background-color:black;
    
} 
```
Y en el p que quieres editar seria por ejemplo:
```html
<p>Es el <i>Ejercicio 7</i> de la  <i>asignatura</i> Aplicaciones WEB </p>
```
En este caso la palabra asignatura aunque este entre <code>i</code> no funciona porque no es el primer hijo directo.<br>
<b>8.-</b>
