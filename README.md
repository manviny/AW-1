# AW
## Actividades HTML y CSS
#### 1. Estructura mínima de una web.
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

#### 2. Explica las 3 formas de usar CSS en HTML.

>**CSS externo**: En la cabecera de HTML, el bloque head. Así, los navegadores sabrán que deben aplicar los estilos del archivo (ejemplo.css) al documento HTML actual.
```html
<link rel="stylesheet" type="text/css" href="ejemplo.css" />
```
>**CSS interno**: Consiste en añadir los estilos directamente en la cabecera HTML del documento. Este sistema puede servir en algunos casos, pero hay que tener en cuenta que utilizándolo, arruinamos la ventaja de tener los estilos en un documento independiente, por lo que siempre es preferible guardarlo en un archivo externo CSS.
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
>**CSS embebido**: Consiste en añadirlo directamente en las propias etiquetas, a través del atributo style.
```html
<p>¡Hola <span style="color:#FF0000">Esto es el ejemplo</span>!</p>
```

#### 3. Crea una lista sin ordenar con 5 ingredientes de una receta de cocina.
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
