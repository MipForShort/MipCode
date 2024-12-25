 
2024-10-22 11:12

Status: #terminado #documentación #fundamentos #sintaxisBasica #C

Tags: [[sintaxisBásica]] [[fundamentos]] [[guías]] [[C]] [[documentación]]
# Estructuras de datos en C

## Arreglos (Array)

Son cadenas secuenciales de caracteres para almacenar elementos. Por lo general son finitos, de no muy grande magnitud y siempre siguen un orden.

## Listas enlazadas (Linked lists)

Son una cadena de nodos que contienen un valor en conjunto de un pointer nulo o que apunte a otro pointer, siendo el nodo final nulo.

![[Captura de pantalla 2024-10-22 112016.png]]

## Tablas hash (Hash tables)

A grandes rasgos, son arreglos de listas enlazadas.

Una buena función hash

- Siempre regresa el mismo valor para el mismo input
- Produce una distribución a través de las llaves
- Utiliza todas las llaves

![[Pasted image 20241022112501.png]]

## Árboles (Tree or Tries)

Son estructuras donde dada una cantidad de datos estas se segmentan manteniendo el orden de los elementos resultando en *padres* e *hijos*. Una forma peculiar es verlos representados como un nodo (padre) apuntando a su respectivo consecutivo (hijo), donde cada nodo padre puede tener hasta dos nodos hijos.

![[Captura de pantalla 2024-10-22 112930.png]]

## Nodos (Nodes)

Código en C de la estructura de nodos en una lista. NOTA: Todo comentario en el código debe ser en inglés

```
/* 
    We create data type struct called node that
    will contain a string and the same struct as
    a pointer to our "next" node
*/
typedef struct node
{
	char *phrase;
	struct node *next;
}
node;

/* 
	We set a NULL pointer called list	
	and also a node n that will be the size
	of a node
*/
node *list = NULL;
node *n = malloc(sizeof(node));

// This is how we can set values to structs
n->phrase = "HI!";
n->next = NULL;

// We currently set list equals to our node so we don't
// loose track of it
list = n;

// Now we set n to another malloc of size node and
// and we set new values but now our next value
// becomes the address of list
n = malloc(sizeof(node));
n->phrase = "Hey!";
n->next = list;

// We set list to n again so now it points to n and
// now it becomes the first item on the list
list = n;

// We set a ptr that points to the next address of list
node *ptr = list->next;

// Free list
free(list);

// Now we set the value from ptr that is left to list again
list = ptr;

// Wee set the pointer to the track of list again so we free it after
ptr = list->next;

free(list);

list = ptr;
```


## Estructuras (Structures)

Las estructuras proveen una manera de unificar variables de diferentes tipo dentro de un único tipo de variable nueva con su propio nombre.

Las estructuras (*structs*) se utilizan para agrupar una variedad de tipos de datos que tengan una conexión lógica.

Piensa sobre una estructura como una *super-variable*.

*Por ejemplo:*

```
struct car
{
	int year;
	char model[10];
	char plate[7];
	int odometer;
	double engine-size;
};

// variable declaration
struct car mycar;

// field accesing;
mycar.year = 2011;
strcpy(mycar.plate, "CS50");
mycar.odometer = 50505;
```

- Una ves que tenemos definida nuestra estructura lo que típicamente se hace es separarla en archivos *.h* separados o al principio de nuestro programa fuera de cualquier función
- Significa que se pueden crear variables del tipo de dato que creamos
- Se puede accesar a varios campos (***fields or members***), de la estructura utilizando el operador    (**.**)

### Pointers a estructuras

Las estructuras, como las variables u otros tipo de datos, no necesitan ser creados en el stack. Se pueden asignar dinámicamente las estructuras en el mismo tiempo que corremos nuestro programa.

Para poder acceder a los campos de la estructura en esta situación, primero necesitamos de-referenciar el pointer a la estructura, después podemos acceder a los campos.

```
// variable declaration
struct car *mycar = malloc(sizeof(struct car));

// field accessing
(*mycar).year = 2011;
strcpy((*mycar).plate, "CS50");
(*mycar).odometer = 50505;

// Another sintax with arrow
```

Existe otro operador más simple que podemos utilizar para simplificar la sintaxis. El operador flecha (->) que hace dos cosas:

- Primero, hace ***dereference*** al pointer de la izquierda del operador
- Segundo, accesa el campo de la derecha del operador

Por lo cual podemos tener el siguiente código:

```
struct car *mycar = malloc(sizeof(struct car));

// field accessing
mycar->year = 2011;
strcpy(mycar->plate, "CS50");
mycar->odometer = 50505;
```
## References
