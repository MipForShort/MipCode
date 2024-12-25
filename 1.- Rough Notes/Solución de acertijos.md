
2024-12-19 10:37

Status: #terminado  #documentación  #fundamentos

Tags: [[documentación]] [[fundamentos]] [[guías]]
# Solución de acertijos

Vamos a resolver un acertijo

|     |     |     |
| --- | --- | --- |
|     |     |     |
|     |     |     |

Tenemos que armar un cuadrado mágico. Debemos usar los dígitos del 1 al 9, de manera que la suma de cada fila, columna y dos diagonales den el mismo resultado.

Qué sucede si decidimos utilizar la siguiente combinación:

| 1   | 2   | 3   |
| --- | --- | --- |
| 4   | 5   | 6   |
| 7   | 8   | 9   |
>Fila 1: 1 + 2 + 3 = 6 
>Fila 2: 4 + 5 + 6 = 15 
>Fila 3: 7 + 8 + 9 = 24
>>Columna 1: 1 + 4 + 7 = 12
>>Columna 2: 2 + 5 + 8 = 15
>>Columna 3: 3 + 6 + 9 = 18
>>>Diagonal 1: 1 + 5 + 9 = 15
>>>Diagonal 2: 7 + 5 + 3 = 15

Disponemos de los siguientes casos a partir de estos resultados.

Miremos como 5 puede quedar en el cuadro del centro porque pues es el medio en la secuencia de 1 a 9.

Otra característica que podemos encontrar es que las diagonales sumadas dan 15. Entonces podemos deducir que 1 + 9 = 7 + 3, ambos dan 10 para después ser sumados con 5.

Entonces podemos elegir diagonales, columna central y fila central para seleccionar parejas que den 10 como resultado de su suma.

| 7   | 6   | 2   |
| --- | --- | --- |
|     | 5   |     |
| 8   | 4   | 3   |
Al llegar a esta solución, o un derivado, podemos quedar con las soluciones *(1, 9) o (9, 1)*.

Existe una propuesta a este cuadrado mágico.

| 4   | 9   | 2   |
| --- | --- | --- |
| 3   | 5   | 7   |
| 8   | 1   | 6   |
Se puede observar que la solución es válida debido a que todas sus filas, columnas y diagonales dan como resultado 15.
## References
