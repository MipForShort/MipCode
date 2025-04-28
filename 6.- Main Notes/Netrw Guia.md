
2025-04-27 18:15

Status: #terminado #documentación #fundamentos #vim 

Tags: [[documentación]] [[fundamentos]]
# Netrw Guia


### ¿Cómo navegar entre archivos y carpetas en netrw?

Aquí lo básico que debes saber:

| Tecla       | Qué hace                                                            |
| ----------- | ------------------------------------------------------------------- |
| `Enter`     | Abrir un archivo o **entrar** a un directorio                       |
| `-` (guion) | **Subir** al directorio padre                                       |
| `h`         | Ayuda (te explica los atajos disponibles)                           |
| `u`         | Subir de carpeta (igual que `-`)                                    |
| `i`         | Cambiar el **modo de vista** (lista detallada, lista simple, árbol) |
| `r`         | **Refrescar** el contenido                                          |
| `%`         | Crear un **archivo nuevo**                                          |
| `d`         | Crear un **directorio nuevo**                                       |
| `D`         | **Borrar** archivo o directorio                                     |
| `R`         | **Renombrar** archivo o directorio                                  |
| `p`         | **Previsualizar** un archivo sin salirte de netrw                   |
| `q`         | Cerrar netrw                                                        |
**Extra:**

- Puedes moverte como en cualquier buffer normal (`j` para bajar, `k` para subir, etc).
    
- Si quieres **abrir un archivo en un split**, puedes:
    
    - `s` → abre en un **horizontal split** (`:split`)
        
    - `v` → abre en un **vertical split** (`:vsplit`)

### ¿Cómo se ve netrw normalmente?

Cuando abres `vim .`, ves algo como:

../
file1.txt
file2.c
folder1/
folder2/

`../` te lleva al directorio anterior.

### Tips pro para usarlo mejor:

- Si quieres que **netrw se abra automáticamente** cuando abres Vim sin archivos, pon esto en tu `~/.vimrc`:


autocmd VimEnter * if argc() == 0 | Explore | endif

_(Así cuando abres Vim sin argumentos, entras directo a la exploración de archivos.)_

- Puedes navegar entre **varios buffers** (`:bnext`, `:bprev`, etc) si abres varios archivos.
    
- Puedes **marcar varios archivos** (`mf`) y después abrirlos todos juntos.
## References
