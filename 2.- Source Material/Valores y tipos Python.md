
2024-12-19 14:42

Status: #terminado #documentación #sintaxisBasica #fundamentos #Python 

Tags: [[documentación]] [[fundamentos]] [[Python]] [[sintaxisBásica]] 
# Valores y tipos Python

Pueden existir varios *tipos* de valores.

Uno son los enteros como: *2*. Otro es una "cadena" de caracteres como ```¡Hola mundo!```. Podemos saber el tipo de valor que manejamos diciéndole al programa lo siguiente:

```
>>> type("¡Hola mundo!")
<type ’string’>
>>> type(30)
<type ’int’>
```

Existen valores llamados flotantes (*float*) que representan números reales o decimales

```
>>> type(5.7)
<type ’float’>
```

¿Qué sucede entonces con valores como *"30"* o *"5.7"*. Parecen números pero encerrados.

```
>>> type("30")
<type ’string’>
>>> type("5.7")
<type ’string’>
```

Son cadenas de texto.

¿Qué sucede entonces con ```print(1,000,000)```?

```
>>> print(1,000,000)
1 0 0
```

Recibimos una respuesta inesperada. Utilizar (,) sin antes encerrar puede traernos problemas dependiendo de lo que se desea obtener.

## References
