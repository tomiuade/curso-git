# Clase 01 - Git desarrollo colaborativo


## Markdown (md)
Un lenguaje de marcas que nos permite crear documentaciones, anotaciones de proyectos.

### Imagen

![markdown](_ref/markdown.png)

### Títulos

# h1
## h2
### h3
#### h4
##### h5
###### h6

### Separador

---

### Listas ordenadas

1. Item
2. Item 
3. Item
4. Item

### Listas desordenadas

* Item 1
* Item 2
* Item 3
* Item 4

### Negrita

Esto es un texto en **negrita**

### Cursiva

Esto es un texto en *cursiva*

### Link

<https://github.com>

## GIT

![git](_ref/git.png)

### Configuración de GIT

#### Agregar un usuario

```sh
git config --global user.name "Maximiliano Principe" # Global (Para todos los repos que se creen en este usuario de windows)

git config --local user.name "Maximiliano Principe" # Local (Para este único repo) Este comando se tique ejecutar luego de haber creado un repo (git init)
```

#### Agregar un correo

```sh
git config --global user.email "mlapeducacionit@gmail.com" # Global (Para todos los repos que se creen en este usuario de windows)

git config --local user.email "mlapeducacionit@gmail.com" # Local (Para este único repo) Este comando se tique ejecutar luego de haber creado un repo (git init)
```

#### Verificar las configuraciones hechas

```sh
git config --global --get-regexp user
```

#### Quitar una propiedad dentro de la configuración

```sh
git config --global --unset user.mail
```

#### Abrir editor para hacer configuraciones manuales

```sh
git config --global -e
```

#### Inicializamos un repositorio de GIT

```sh
git init # Va a crear en la carpeta del proyecto una directorio '.git' dentro
```

**NOTA**: NO hay que borrar la carpeta .git, ni hay que modiicar los archivos dentro de ella. Solo trabajar git sobre ese directorio, no nosotros

#### Limpiar consola

```sh
clear # windows
cls # linus
# ctrl + l
```

#### GIT STATUS ####
¿Que hace? Verifica el estado de los archivos y en que area (o en que parte de la estructura virtual) están los archivos

* UNTRACKED: Que los archivos aún están en el working directory (WD) y no están siendo seguidos (controlados) por GIT.

* STAGED: Archivos que están preparados para crear un commit (Sacar la foto) El snapshot y preservar los cambios hechos de mi código fuente. (PRE FOTO) MODIFICACIÓN

* UNMODIFIED: Los archivos que están en este estado no fueron modificados respecto del archivo/s que esta en Local Repo (LR). Respecto a la foto que tenía en el Local Repo

* MODIFIED: Los archivos que están modificados respecto del estado actual del Local Repo (LR)

* cambios extraños que hay en mi








