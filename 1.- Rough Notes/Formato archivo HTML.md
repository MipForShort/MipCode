
2024-10-19 13:44

Status: #enProceso #html #documentación #sintaxisBasica

Tags: [[html]] [[sintaxisBásica]] [[programaciónWeb]] [[guías]] [[documentación]]
# Formato archivo HTML

Para escribir el nombre de una etiqueta es necesario abrir y cerrar la etiqueta. 

```
	<tag> TEXTO </tag>
```

Todo lo que esté dentro de la etiqueta es a lo que se va aplicar el formato de la etiqueta que hayamos determinado.

## Estructura

Una estructura sencilla de una página HTML es la siguiente: 

```
	<!DOCTYPE html>

	<html>
	    <head>
	        <title>Título</title>
	    </head>
	    <body>
	       
	    </body>
	</html>
```

## Encabezados

Para determinar títulos en HTML podemos usar la etiqueta h y consiguiente del numero que queremos agregar hasta 6.

```
	<h1>Título</h1>
	<h2>Subtitulo</h2>
```

Por página para mejor SEO es únicamente utilizar la etiqueta h1 solamente una vez.
## Párrafos

Un párrafo se puede utilizar con la etiqueta (p):

```
<p> Lorem ipsum dolor sit amet consectetur adipisicing elit. Itaque quidem illo voluptates quas inventore earum doloribus nemo, sed sint. Praesentium sapiente quidem necessitatibus corporis nisi voluptate nesciunt explicabo omnis qui. </p>	
```

## Listas

Tenemos dos tipos de listas, ordenadas y desordenadas. La sintaxis de una lista es la siguiente:

```
	<ul>
		<li>Elemento 1</li>
		<li>Elemento 2</li>
		<li>Elemento 3</li>
	</ul>
	<ol>
		<li>Elemento 1</li>
		<li>Elemento 2</li>
		<li>Elemento 3</li>
	</ol>
```

Donde la etiqueta (ol) es una lista ordenada y (ul) una lista desordenada. Es importante saber qué tipo de lista utilizar dependiendo del orden de los elementos.
## References
