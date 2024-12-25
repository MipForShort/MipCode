
2024-10-16 11:54

Status: #terminado #sintaxisBasica #fundamentos #documentación #markdown

Tags: [[Markdown]] [[guías]] [[sintaxisBásica]] [[fundamentos]] [[documentación]]
# Sintaxis básica de Markdown

Hay varios motores para utilizar ***Markdown*** en donde podremos utilizar distintos elementos dentro de nuestros textos.

A continuación se pondrán los distintos elementos que existen para el lenguaje ***Markdown***.
## Encabezados (Headings)

Para poder crear un ***header*** o encabezado podemos utilizar el carácter (#) antes del texto el cual planeamos utilizar. El número de signos corresponden al nivel de encabezado que vayamos utilizar. *Por ejemplo:* Si queremos utilizar un encabezado (h3), podemos utilizar tres signos para asignarlo ( ### header).
### Mejores practicas de encabezados

Las aplicaciones de ***Markdown*** no manejan realmente si poner un espacio después del signo para diferenciar un encabezado, así que la mejor manera es colocar un espacio después de los signos que utilicemos.

>***Haz esto***
>># Aquí va el Encabezado
>***No hagas esto***
>>#Aquí va el Encabezado

## Párrafos (Paragraphs)

Para crear párrafos sólo utiliza texto plano para poder hacerlo.

## Quiebres de línea

Se pueden utilizar dos espacios en blanco antes de un quiebre de línea para esta aplicación, pero la mayoría de aplicaciones de ***Markdown*** no tienen un carácter especial para significar una línea nueva así que lo mejor para esto es no utilizar doble espacio debido a que puede ser interprete de errores. Lo más correcto es no utilizar estos quiebres.

## Énfasis

Se pueden añadir tipos de énfasis al texto como **negritas** o *itálicas*.
### Negritas (Bold)

Para poder hacer el texto negritas, es necesario encerrar en doble asterisco nuestro texto. *Por ejemplo:* **Texto**.
### Itálicas

Para poder hacer el texto itálicas podemos encerrar en asterisco sencillo nuestro texto. *Por ejemplo*.
### Negritas e Itálicas

Para poder hacer el texto negritas e itálicas podemos encerrar en triple asterisco nuestro texto. *Por ejemplo:* ***Texto***.
## Bloques de cita (Blockquotes)

Para crear un bloque de cita es necesario poner un > al principio del párrafo.

>***Este es un bloque de citas***

### Bloques de citas con múltiples párrafos

Los ***blockquotes*** pueden contener múltiples párrafos si añadimos  > entre cada línea del ***blockquote***.

>***Este es el primer párrafo***
>
>***Este es el segundo párrafo***

### Bloques de cita anidados

Los bloques de cita pueden ser anidados añadiendo un > al principio del párrafo que ya sea un bloque.

>Bloque Uno
>>Bloque Dos
>>> Bloque Tres

### Mejores prácticas de bloques de citas

Para compatibilidad es mejor mantener los bloques de cita separados por una línea nueva al principio y al final del bloque.

## Listas

La información se puede organizar en listas ordenadas y desordenadas.
### Listas ordenadas

Para crear una lista ordenada podemos escribir un número al inicio de una línea nueva. Pero para mejor práctica es mantener el orden propio de los elementos.

1. Primer Elemento
2. Segundo Elemento
3. Tercer Elemento
### Listas desordenadas

Para poder crear una lista desordenada podemos utilizar los siguientes signos (-, asterisco, +), al frente de una nueva línea.

- Primer Elemento
- Segundo Elemento
- Tercer Elemento

### Mejores practicas de listas

Las mejor practica para escribir listas ordenadas es mantener el orden de los elementos. Para las listas desordenadas es mantener el símbolo que se utiliza en la lista.

## Bloques de código

Para hacer notar el texto como código es simplemente necesario encerrar en comillas invertidas el texto. *Por ejemplo:* `texto`


## Enlaces (Links)

Para crear enlaces se tiene que encerrar el texto en corchetes ([]) y después añadir el URL entre paréntesis. *Por ejemplo:* [Duck Duck Go](https://duckduckgo.com)

### Añadir títulos al enlace

Se pueden añadir títulos al enlace, que se muestran como texto al posicionarnos sobre el vínculo, simplemente añadiendo nuestro título encerrado entre comillas dobles después del URL. *Por ejemplo:* [Duck Duck Go](https://duckduckgo.com "El Mejor navegador web en privacidad")

### URL y correo electrónico

Podemos encerrar entre <> el URL o correo que deseemos utilizar para darle formato a nuestro texto.

### Dar formato a enlaces

Podemos dar formato a los enlaces con los diferentes símbolos que hemos utilizado en este documento. 

*Por ejemplo:*

```
I love supporting the **[EFF](https://eff.org)**.
This is the *[Markdown Guide](https://www.markdownguide.org)*.
See the section on [`code`](#code).
```

*Esto se traduce a:*

I love supporting the **[EFF](https://eff.org)**.
This is the *[Markdown Guide](https://www.markdownguide.org)*.
See the section on [`code`](#code).

### Enlaces de estilo referencia

Estos son un tipo especial de enlaces que se pueden construir y constan de dos partes.

- La primer parte se compone del label o nombre del enlace 
	- ```[enlace]```
- La segunda parte se compone del enlazador
	- ```[1]```

Para darle formato a la segunda parte es necesario añadir en un punto el URL de la siguiente forma:

```
[1]: <https://duckduckgo.com>
```

Ahora para hacer uso de ello tan solo hay que escribir de la siguiente forma nuestro enlace donde planeemos utilizarlo:

```
[duck duck go][1]
[1]: <https://duckduckgo.com>
```

## Imágenes

Para añadir una imagen es necesario añadir un signo de admiración (!) seguido del enlace a la imagen que se utilizará. Esto puede ser escrito como rutas de archivos o URL de internet.

*Por ejemplo:*

```
![The San Juan Mountains are beautiful!](/assets/images/san-juan-mountains.jpg "San Juan Mountains")
```
## References

- [Basic Syntax](https://www.markdownguide.org/basic-syntax/#lists-1)