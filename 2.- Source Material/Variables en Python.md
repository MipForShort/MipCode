
2024-12-19 15:00

Status: #terminado #documentación #sintaxisBasica #fundamentos #Python 

Tags: [[documentación]] [[fundamentos]] [[Python]] [[sintaxisBásica]] 
# Variables en Python

Una característica poderosa de los lenguajes de programación es la capacidad de manipular variables.

Mediante la asignación podemos referir con un nombre a un valor.

```
message = "¿Qué Onda?"
n = 17
pi = 3.14159
```

En papel es común señalar con una flecha el nombre de la variable apuntando hacia el valor, esto es un diagrama de estado.

```
message -> "¿Qué Onda?"
n -> 17
pi -> 3.14159
```

La sentencia ```print()``` también funciona con variables.

```
print(message)
¿Qué Onda?
print(n)
17
print(pi)
3.14159
```

Las variables también tienen tipos.

```
type(message)
<class 'str'>
type(n)
<class 'int'>
type(pi)
<class 'float'>
```

## Nombres de variables y palabras reservadas

A menudo se escriben nombres significativos que especifiquen el uso de la variable. Pueden ser largos, contener letras y números aunque tienen que empezar con una letra. Las mayúsculas son legales aunque por convención no se hace. Si bien ```Pedro y pedro``` son diferentes debido a la capitalización.

El carácter (*_*) puede aparecer en un nombre. A menudo como separador de palabras.

No empezar con una letra y contener símbolos ilegales son errores de sintaxis.

```
5vegeta
SyntaxError: invalid decimal literal
mas$
SyntaxError: invalid syntax
class = "Introducción a la programación"
SyntaxError: invalid syntax
```

¿Qué sucede con ```class```? Esta es una palabra reservada del lenguaje. Estas definen reglas e instrucciones del lenguaje y su estructura, no se pueden usar como nombres de variables.

Algunas palabras reservadas son las siguientes:

```
| and    | continue | else    | for    | import | not   |
| assert | def      | except  | from   | in     | or    |
| break  | del      | exec    | global | is     | pass  |
| class  | elif     | finally | if     | lambda | print |
| raise  | return   | try     | while  |        |       |
```

| and    | continue | else    | for    | import | not   |
| ------ | -------- | ------- | ------ | ------ | ----- |
| assert | def      | except  | from   | in     | or    |
| break  | del      | exec    | global | is     | pass  |
| class  | elif     | finally | if     | lambda | print |
| raise  | return   | try     | while  |        |       |
## References
