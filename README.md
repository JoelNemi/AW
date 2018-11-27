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
Hay mas pseudoclases con mas opciones.
<!DOCTYPE html>
<html>
<head>
</head>
<body>
<table>
  <tbody><tr>
    <th>Selector</th>
    <th>Ejemplo</th>
    <th>Descripción</th>
  </tr>
  <tr>
    <td>:active</td>
    <td>a:active</td>
    <td>Influye a los links activos</td>
  </tr>
  <tr>
    <td>:checked</td>
    <td>input:checked</td>
    <td>Influye cada elemento <code>input</code> marcado</td>
</td>
  </tr>
  <tr>
    <td>:disabled</td>
    <td>input:disabled</td>
    <td>Influye cada elemento <code>input</code> marcado</td>
  </tr>
  <tr>
    <td>:empty</td>
    <td>p:empty</td>
    <td>Influye a todas las <code>p</code> que no tiene hijos</td>
  </tr>
  <tr>
    <td>:enabled</td>
    <td>input:enabled</td>
    <td>Influye a todos los elementos <code>input</code></td>
  </tr>
  <tr>
    <td>:first-child</td>
    <td>p:first-child</td>
    <td>Influye a todos los <code>p</code> que sean primer hijos</td>
  </tr>
  <tr>
    <td>:first-of-type</td>
    <td>p:first-of-type</td>
    <td>Influye cada elemento <code>p</code> que sea el primer elemento <code>p</code> de su padre</td>
  </tr>
  <tr>
    <td>:focus</td>
    <td>input:focus</td>
    <td>Influye en el elemento <code>input</code> que esta seleccionado</td>
  </tr>
  <tr>
    <td>:hover</td>
    <td>a:hover</td>
    <td>Influye a los links o otro elemento que tenga el raton encima</td>
  </tr>
  <tr>
    <td>:in-range</td>
    <td>input:in-range</td>
    <td>Influye a los elementos <code>input</code> con un valor dentro de un rango especificado</td>
  </tr>
  <tr>
    <td>:invalid</td>
    <td>input:invalid</td>
    <td>Influye a todos los elementos <code>input</code> con un valor no válido</td>
  </tr>
  <tr>
    <td>:lang(<i>language</i>)</td>
    <td>p:lang(EJ7)</td>
    <td>Influye cada elemento <code>p</code> con un valor de atributo lang que comience con "EJ7"</td>
  </tr>
  <tr>
    <td>:last-child</td>
    <td>p:last-child</td>
    <td>Influye a cada elemento <code>p</code> que es el último hijo de su padre</td>
  </tr>
  <tr>
    <td>:last-of-type</td>
    <td>p:last-of-type</td>
    <td>Selecciona cada elemento <code>p</code> que es el último elemento <code>p</code> de su padre</td>
  </tr>
  <tr>
    <td>:link</td>
    <td>a:link</td>
    <td>Influye a todos lo links o otro elemento no visitado</td>
  </tr>
  <tr>
    <td>:not(selector)</td>
    <td>:not(p)</td>
    <td>Influye a cualquier elemento que no sea <code>p</code></td>
  </tr>
  <tr>
    <td>:nth-child(n)</td>
    <td>p:nth-child(2)</td>
    <td>Influye a cada elemento <code>p</code> que sea el segundo hijo de su padre</td>
  </tr>
  <tr>
    <td>:nth-last-child(n)</a></td>
    <td>p:nth-last-child(2)</td>
    <td>
Influye a cada elemento <code>p</code> que es el segundo hijo de su padre, contando desde el último hijo</td>
  </tr>
  <tr>
    <td>:nth-last-of-type(n)</td>
    <td>p:nth-last-of-type(2)</td>
    <td>Influye a cada elemento <code>p</code> que es el segundo elemento <code>p</code> de su padre, contando desde el último hijo</td>
  </tr>
  <tr>
    <td>:nth-of-type(n)</td>
    <td>p:nth-of-type(2)</td>
    <td>Influye a cada elemento <code>p</code> que sea el segundo elemento <code>p</code> de su padre</td>
  </tr>
  <tr>
    <td>:only-of-type</td>
    <td>p:only-of-type</td>
    <td>Influye a  cada elemento <code>p</code> que sea el único elemento <code>p</code> de su padre</td>
  </tr>
  <tr>
    <td>:only-child</td>
    <td>p:only-child</td>
    <td> Influye a cada elemento <code>p</code> que es el único hijo de su padre</td>
  </tr>
  <tr>
    <td>:optional</td>
    <td>input:optional</td>
    <td>Influye a elementos <code>input</code> sin atributo "requerido"</td>
  </tr>
  <tr>
    <td>:out-of-range</a></td>
    <td>input:out-of-range</td>
    <td>Influye a elementos <code>input</code> con un valor fuera de un rango especificado</td>
  </tr>
  <tr>
    <td>:read-only</td>
    <td>input:read-only</td>
    <td>Influya a elementos <code>input</code> con un atributo "readonly" especificado</td>
  </tr>
  <tr>
    <td>:read-write</td>
    <td>input:read-write</td>
    <td>Influya a elementos <code>input</code> sin atributo "readonly"</td>
  </tr>
  <tr>
    <td>:required</td>
    <td>input:required</td>
    <td>Selecciona los elementos <code>input</code> con un atributo "requerido" especificado</td>
  </tr>
  <tr>
    <td>:root</td>
    <td>root</td>
    <td>Influye a la raiz del documento</td>
  </tr>
  <tr>
    <td>:target</td>
    <td>#news:target</td>
    <td>Inflye al elemento activo actual #news (se hace clic en una URL que contiene ese nombre de clase)</td>
  </tr>
  <tr>
    <td>:valid</td>
    <td>input:valid</td>
    <td>Influye a todos los elementos <code>input</code> con un valor válido</td>
  </tr>
  <tr>
    <td>:visited</td>
    <td>a:visited</td>
    <td>Influye a los elementos que ha sido visitado</td>
  </tr>
</tbody></table>
</body>
</html>

</body>
</html>
<b>8.-Explica el modelo de caja de CSS (margin, border y padding)</b><br>
El modelo de caja de CSS se basa en que en cada elemento contiene un conjunto de elementos que le rodean.<br>
Esos elementos son, el mas externo es el margin, que limpia lo que haya en un area x por fuera del Border,<br>
despues esta el Border, que esta alrededor del contenido, a continuacion esta <br>
el padding, que es lo que hay entre el border y el contenido, se usa para desplazar y colocar<br>
a tu gusto el contenido dentro del border.Y por ultimo el contenido, que es basicamente lo hayas colocado,<br>
ya sea un DIV,<br> una imagen o lo que sea.

<b>9.-Explica que son los selectores de CSS y pon ejemplos</b>
