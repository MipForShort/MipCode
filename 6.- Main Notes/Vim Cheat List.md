
2025-04-26 14:51

Status: #terminado #documentación #fundamentos #vim

Tags: [[documentación]] [[fundamentos]]
# Vim Cheat List

## Movimientos básicos
- `h` : Mover cursor a la izquierda
- `l` : Mover cursor a la derecha
- `j` : Mover cursor hacia abajo
- `k` : Mover cursor hacia arriba
- `w` : Saltar al inicio de la siguiente palabra
- `e` : Saltar al final de la palabra actual
- `b` : Saltar al inicio de la palabra actual
- `0` : Ir al inicio de la línea
- `^` : Ir al primer carácter no vacío de la línea
- `$` : Ir al final de la línea
- `gg` : Ir al inicio del archivo
- `G` : Ir al final del archivo
- `:n` : Ir a la línea `n`

## Modos
- `i` : Insertar texto antes del cursor
- `I` : Insertar al inicio de la línea
- `a` : Insertar texto después del cursor
- `A` : Insertar al final de la línea
- `o` : Insertar una nueva línea debajo
- `O` : Insertar una nueva línea encima
- `Esc` : Volver al modo normal

## Edición
- `x` : Eliminar el carácter bajo el cursor
- `dd` : Eliminar (cortar) la línea actual
- `yy` : Copiar la línea actual
- `p` : Pegar después del cursor
- `P` : Pegar antes del cursor
- `u` : Deshacer
- `Ctrl + r` : Rehacer
- `cw` : Cambiar la palabra desde el cursor
- `ci"` : Cambiar el contenido entre comillas (similares comandos con `()`, `{}`, etc.)
- `>>` : Indentar la línea actual
- `<<` : Desindentar la línea actual

## Buscar y reemplazar
- `/texto` : Buscar "texto" hacia abajo
- `?texto` : Buscar "texto" hacia arriba
- `n` : Ir a la siguiente coincidencia
- `N` : Ir a la coincidencia anterior
- `:%s/viejo/nuevo/g` : Reemplazar todas las ocurrencias de "viejo" por "nuevo"
- `:noh` : Quitar el resaltado de búsquedas

## Archivos
- `:w` : Guardar cambios
- `:q` : Salir
- `:wq` : Guardar y salir
- `:q!` : Salir sin guardar
- `:e nombre_archivo` : Abrir un archivo
- `:bn` : Ir al siguiente buffer (archivo)
- `:bp` : Ir al buffer anterior

## Ayuda
- `:help` : Abrir ayuda de Vim
- `:help comando` : Obtener ayuda sobre un comando específico

## Combinaciones útiles
- `Ctrl + d` : Avanzar media pantalla hacia abajo
- `Ctrl + u` : Retroceder media pantalla hacia arriba
- `Ctrl + f` : Avanzar una pantalla completa
- `Ctrl + b` : Retroceder una pantalla completa
- `zz` : Centrar la línea actual en la pantalla

---

¡Práctica y verás que pronto te sentirás a gusto con Vim!





## References
