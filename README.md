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
La segunda forma es en un <style> dentro del elemento <head> <br>
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
3.-
