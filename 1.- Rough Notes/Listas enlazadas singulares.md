
2024-10-24 11:10

Status: #enProceso #documentación #C  #fundamentos #sintaxisBasica

Tags: [[sintaxisBásica]] [[documentación]] [[C]] [[fundamentos]]
# Listas enlazadas singulares

Una combinación de nodos es una lista enlazada, donde se necesitan dos miembros:

- Datos de algún tipo de datos (int, char, float...)
- Un pointer hacia otro nodo del mismo tipo

De esta manera se pueden crear un set de nodos que pueden ser pensados como una cadena de elementos que se sigue de principio a fin.

```
typedef struct sllist
{
	VALUE val;
	struct sllist* next;
}
sllnode;
```


## References
