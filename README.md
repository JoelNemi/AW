# AW
## Paginas Web
1.-Estructura mínima de una web
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
2.-Explica las 3 formas de usar CSS en HTML <br>
La primera forma es en la misma linea<br>
-Ejemplo:
```html
	<p style="color:blue;">Ejemplo de CSS en la misma linea</p>
```
La segunda forma es en un <style> dentro del elemento "head" <br>
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
Por ultimo crear un archivo CSS y enlazarlo con el html
#Ejemplo:
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
3.-Crea una lista sin ordenar con 5 ingredientes de una receta de cocina
```html
<ul>
	<li>arina</li>
	<li>Limón</li>
	<li>Pimienta</li>
	<li>Sal</li>
	<li>Ajo</li>
</ul>
```
4.-Como se puede incluir javascript en HTML <br>
 Se incorpora con la etiqueta <script>
```html
	<script>
	document.getElementById("Prueba").innerHTML = "Prueba JavaScript";
</script>
```
5.-¿Que diferencia hay entre una clase y una ID <br>
	Una clase engloba varios elementos para que tengan el mismo codigo CSS, "p" y "h2" pueden tener la misma clase, <br>
	en cambio un ID solo puede haber un ID unico que pertenezca a un elemento aparte el Id diferencia entre minusculas y <br> 
	mayusculas, y no puede contener un espacio ni tabulaciones, al conterio que una clase.<br>
6.-Código para hacer un enlace a otra página y que esta se abra en una nueva ventana
```html
<a href="https://www.google.com" target="_blank">Ejercicio 6</a> 
```
7.-¿Qué son las pseudoclases?, pon ejemplos.<br>
