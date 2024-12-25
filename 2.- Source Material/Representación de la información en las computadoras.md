
2024-12-14 16:14

Status: #terminado #documentación  #fundamentos 

Tags: [[documentación]] [[fundamentos]]
# Representación de la información en las computadoras

## Textos

Existen las siguientes maneras de texto en la computadora:

1. Caracteres alfabéticos

![[Pasted image 20241214161706.png]]

2. Caracteres numéricos

![[Pasted image 20241214161727.png]]

3. Caracteres especiales

![[Pasted image 20241214161747.png]]

4. Caracteres geométricos y gráficos

![[Pasted image 20241214161825.png]]

5. Caracteres de control

Existen códigos o codificaciones en la computación donde se asignan a un caracter *n* cantidad de bits.

- Código EBCDIC (Extended Binary Coded Decimal Inter Change Code)
	- Utiliza *n* = 8 bits hasta *m* = 2^8 = 256 bits
- Código ASCII (American Standard Code for Information Interchange)
	- Utiliza 7 bits y permite representar 128 caracteres.
- Código Unicode
	- Utiliza un patrón único de 16 bits que permite hasta 2^16 bits o 65,536 patrones de bits diferentes

## Números

### Enteros

Se representan con notación binaria, normalmente se almacenan en 2 *bytes*. Por ejemplo

- 1000 1110 0101 1011
### Reales

Son aquellos que contienen parte decimal. Se conocen en algunos lenguajes como *floats*.

Existen dos formas de representar números reales. La primera es con notación del punto decimal.

![[Pasted image 20241214162954.png]]

La segunda es con notación científica o exponencial.

![[Pasted image 20241214163030.png]]

### Caracteres

Un documento de texto se escribe con caracteres de un código, comunmente ASCII o Unicode.

En C++ se pueden categorizar como un *char*. Lo cual es un código numérico que se almacena en un byte.

## Imágenes

Una imagen se representa por patrones de bits, generados por un periférico de entrada (cámaras, escáner, etc.)

![[Pasted image 20241215175844.png]]
*Tabla de tipos enteros reales, en C++*

Existen dos formas de representar imágenes:

- Mapas de bits, que son una colección de puntos llamados *pixeles*. Cada color se puede representar por una cadena de bits o patrón donde cada bit resulta en el color a mostrar en pantalla.
- Mapas de vectores, estos descomponen la imagen en una colección de objetos como líneas, polígonos y textos con sus respectivos detalles o atributos.

![[Pasted image 20241214163637.png]]
*Mapa de bits*

![[Pasted image 20241214163706.png]]
*Mapa de vectores*

## Sonidos

La manera más común es mostrando la amplitud de la onda de sonido en intervalos regulares y registrar las series en valores. Se captan mediante micrófonos o dispositivos similares. Produce una señal analógica que se recoge mediante muestras a través del tiempo que dan datos que se procesan a través de la digitalización a secuencias de bits.
## References
