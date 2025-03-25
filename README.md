#Proyecto GitFlow PHP Pedro

# Documentación del Flujo de Trabajo con Git Flow

Pasos seguidos (sin incluir las direcciones de los archivos):

---
## Parte 1: Configuración Inicial

1. Se ha creado el repositorio en GitHub.
2. Se ha clonado el repositorio con el comando:
   ```sh
   git clone <URL_DEL_REPOSITORIO>
   ```
3. Se ha creado este archivo `README.md` y se ha subido a la rama `main`.
4. Se han utilizado los comandos:
   ```sh
   git add .
   git commit -m "Añadiendo README.md"
   git push origin main
   ```
5. Se ha creado la rama `develop`.
6. Se ha inicializado Git Flow con:
   ```sh
   git flow init
   ```

---
## Parte 2: Creación de una Nueva Funcionalidad

1. Se ha creado la nueva funcionalidad con el comando:
   ```sh
   git flow feature start crear-mi-archivo
   ```
2. Se ha creado una carpeta `alumnos/` y dentro de ella un archivo `alumno.php`.
3. Se han agregado los cambios y confirmado en la rama `develop`:
   ```sh
   git add .
   git commit -m "Añadiendo alumno.php"
   git push origin feature/crear-mi-archivo
   ```

---
## Parte 3: Modificación del Index

1. Se ha creado una nueva funcionalidad en Git Flow con el comando:
   ```sh
   git flow feature start modificar-index
   ```
2. Se ha creado un archivo `index.php` y se ha agregado contenido.
3. Se han confirmado los cambios y la funcionalidad se ha subido a `develop`:
   ```sh
   git add .
   git commit -m "Añadiendo index.php"
   git push origin feature/modificar-index
   ```
---

## Parte 4: Eliminación de un Archivo

1. Se ha eliminado un archivo con el comando:
   sh
   git rm alumnos/alvaro.php
   
2. Se han agregado los cambios y se han confirmado:
   ```sh
   git add .
   git commit -m "Eliminando archivo alumnos/Pedro.php"
   git push origin develop
   
## Parte 5: Publicación de una Versión Final

Para subir una versión estable, se han ejecutado los siguientes comandos:
```sh
git flow release start v1.0
git flow release finish v1.0

git push origin main
git push origin develop
git push origin --tags
```


