# Clase 02 

## .gitkeep
Archivo para preservar una carpeta vacía dentro del repositorio de git. Creo el archivo en la carpeta que quiero mantener

## .gitignore
Es archivo que me permite descartar archivos que no formen parte de mi repo. Normalmente se crea en el directorio raíz del proyecto.

## GIT Status
Nos permite visualizar el estado actual de los archivos dentro de la dinamica de GIT

```sh
git status
git status -s # git status --short
```

## GIT DIFF
Me permite comparar entre el working directory y el staged o entre el staged y el local repo. Etc...

```sh
git diff # Compara el working directory contra el staged
```

```sh
git diff --staged # Compara el staging area contra el local repo
```

## GIT LOG 
Me permite ver el listado de commits realizados. El timeline de commit (snapshot) sacadas.

```sh
git log # forma larga
git log --oneline # forma corta
```

## GIT ADD
Me permite agregar a la zona de staging area (area de confirmación) los cambios que quiera guardar proximamente en un commit (Zona de pre foto para luego sacar la foto)

```sh
git add <que-cosas-quiero-guardar-en-el-stage>
git add . # Todos los archivos
git add <nombre-archivo> <nombre-archivo>
git add README.md .gitignore # Ejemplo

git add --patch # Me permite elegir que cambios en la líneas quiero agregar en el staging area

# y -> Agrega el hunk (zona de staging)
# n -> No lo agregar al hunk (zona de staging)
# s -> Dividir hunk a colocar en el staging
# e -> Manual (elijo usando el numeral '#' que cosa quiero no colocar en el staging)
```

## GIT RESTORE
Me permite recuperar los archivos desde el historico de cambios de git

```sh
git restore . # Me recupera todos los archivos basado en el último commit
git restore <nombre-archivo>
git restore clase.02/README.md
git restore --staged <nombre-archivo> # Saco del staging area y dejo en el working directory
git restore --staged clase.02/README.md
```

## GIT COMMIT
Me permite sacar una foto de lo que tengo en la zona de staging area. Foto para preservar los cambios en el timeline de commits. En la historia del proyecto.

```sh
git commit -m "<mensaje-descriptivo>" # -m: mensaje

git commit -am "<mensaje-descriptivo>" # -m: mensaje -a: add (Cuando el archivo esta siendo seguido por git - modified)
```

## Empezar a trabajar con el remoto
Nosotros vamos a tener un repositorio local (.git) y vamos a tener que trabajar también en un un repositorio remoto (GitHub, GitLab, BitBucket)

### GIT PUSH
Para subir los cambios del repositorio local al remoto

### GIT FETCH
Me sirven para solicitar los cambios que ocurrieron en el remoto pero sin traer esos cambios

### GIT PULL
Me sirven para traerme los cambios del remoto al local
