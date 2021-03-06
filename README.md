# AW
## Actividades HTML y CSS
### 1. Estructura mínima de una web.
```html
<!DOCTYPE  html>
<html>
	<head>
		<title>Título de la página</title>
	</head>
	<body>
	</body>
</html>
```
>**html**: Este elemento envuelve todo el contenido de la página.

>**head**: Este elemento designa la parte de encabezado del documento. Puede incluir información opcional sobre la página Web, como puede ser el título (el navegador lo muestra en la barra de título), palabras clave de búsqueda opcionales...

>**body**: Este elemento alberga el contenido de su página Web, es decir, aquello que queremos que aparezca en el área de navegación del navegador.

### 2. Explica las 3 formas de usar CSS en HTML.

-**CSS externo**: En la cabecera de HTML, el bloque **head**. Así, los navegadores sabrán que deben aplicar los estilos del archivo (ejemplo.css) al documento HTML actual.
```html
<link rel="stylesheet" type="text/css" href="ejemplo.css" />
```
-**CSS interno**: Consiste en añadir los estilos directamente en la cabecera HTML del documento. Este sistema puede servir en algunos casos, pero hay que tener en cuenta que utilizándolo, arruinamos la ventaja de tener los estilos en un documento independiente, por lo que siempre es preferible guardarlo en un archivo externo CSS.
```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo</title>
    <style type="text/css">
        div {
            background:#FFFFFF;
        }
    </style>
</head>
```
-**CSS embebido**: Consiste en añadirlo directamente en las propias etiquetas, a través del atributo **style**.
```html
<p>¡Hola <span style="color:#FF0000">Esto es el ejemplo</span>!</p>
```

### 3. Crea una lista sin ordenar con 5 ingredientes de una receta de cocina.
```html
<!DOCTYPE  html>
<html>
	<head>
		<title>Título de la página</title>
	</head>
	<body>
		<ul>
			<li>Arina</li>
			<li>Azucar</li>
			<li>Huevo</li>
			<li>Cacao</li>
			<li>Leche</li>
		</ul>
	</body>
</html>
```

### 4. Como se puede incluir javascript en HTML.
La primera forma es añadiendo Java Script directamente a un documento HTML, se puede hacer utilizando la etqueta **script**, se puedfe agregar entre las etiquetas **head** o **body**. De normal se recomienda entre **head** para que este separado del contenido del archivo HTML, pero colocarlo entre **body** puede ayudar a mejorar la velocidad de carga.
```html
<!DOCTYPE  html>
<html>
	<head>
		<title>Título de la página</title>
	
			<script>JAVASCRIPT SUELE IR AQUI</script>
	
	</head>
	<body>
		<script>JAVASCRIPT TAMBIEN PUEDE IR AQUI</script>
	
	</body>
</html>
```
También se puede agregar el código JavaScript a un archivo separado, a veces insertarlo de forma directa no es la mejor opción porque algunos scripts deben utilizarse en varias páginas, por eso es mejor mantener el codigo en archivos separados.
```html
<!DOCTYPE  html>
<html>
	<head>
		<title>Título de la página</title>
	</head>
	<body>
		<script src="ejemploJS.js"></script>
	</body>
</html>
```

### 5. ¿Que diferencia hay entre una clase y una ID?
Los **id** están pensados para que el elemento que se selecciona sea único. Las **clases** están pensadas para poder definir el mosmo estilo a varios elementos de la página.

### 6. Código para hacer un enlace a otra página y que esta se abra en una nueva ventana.
```html
<a href="http://blog.elinsti.com" target="_blank">Enlace de ejemplo</a>
```

### 7. ¿Qué son las pseudoclases? Pon ejemplos.
Las pseudoclases son unas palabras clave que se añaden a los selectores y especifican un estado especial del elemento seleccionado. Ejemplos, **:hover** que permite saber si el ratón está encima de un elemento o no, cambiendo el estilo del elemento especificado por el selector. **:visited** historial de navegación, **:checked** estado de su contenido en algunos elementos de formulario, **:link** representa un elemento que aun no se ha vistado,.etc.
```html
div:hover {
  background-color: red;
}
```

### 8. Explica el modelo de caja de CSS (margin, border y padding).
El modelo de las cajas es la base del diseño Web, cada elemento se representa como una caja rectangular con el contenido, margin, padding y border contruidos uno sobre otro como capas.

>**Padding**: Hace referencia al margen interior de la caja CSS, entre el limte exterior de la caja del contenido y el limite interior del border.

>**Border**: Entre el limite exterior del padding y el limite interior del margin. Por defecto tiene un tamaño 0, pero podemos cambiar su grosor, color y estilo.

>**Margin**: Es lo que envuelve la caja CSS y sostiene las otras cajas de diseño. Su comportamiento es parecido al del padding.

### 9. Explica que son los selectores de CSS y pon ejemplos.
Los selectores CSS son patrones que se utilizan para seleccionar los elementos que se quieren aplicar un estilo.
Ejemplos:
```html
div > p --> Selecciona todos los elementos <p> donde el padre sea un elemento <div>.
```
```html
h1, p --> Aplica estilo a todos los elementos <h1> y a todos los elementos <p>.
```
```html
a[target=_blank] --> Selecciona todos los elementos <a> con target = "_ blank".
```
```html
a:link --> Selecciona y pon un estiloa los enlaces no visitados.
```
```html
a:visited --> Seleccione y pon un estilo a los enlaces visitados.
```

### 10. Di a quien afectan.
```html
p a { color: red; } --> Poner en rojo los enlaces <a> que esté dentro de los elementos <p>.
```
```html
p > a { color: red; } -->  Poner en rojo los enlaces <a> donde el padre sea un elemento <p>.
```
```html
h1 + h2 { color: red } --> Poner en rojo cada elemento <h2> que se esté inmediatamente después del elemnto <h1>.
```
```html
a[class] { color: blue; } --> Poner en azul a todos los enlaces <a> con el atrubuto class.
```
```html
a[class="externo"] { color: blue; } --> Poner en azul todos los enlaces <a> con el atrubuto class con el valor "externo".
```
```html
a[href="http://www.ejemplo.com"] { color: blue; } --> Poner en azul todos los enlazes <a> que vayan a la direccion "http://www.ejemplo.com".
```
