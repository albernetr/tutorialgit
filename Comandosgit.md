# Comandos de Git

**Descripción:** Este archivo contiene los comando basicos para utilizar git.

## Convenciones:#
 <> : Significa que esta informacion debe ser agregada por el usuario.

 Mayusculas: Indica que esta informacion es agregada por el usuario y puede ser utilizada en varios lugares, pueden ser datos como nombres de usuarios, rutas de archivos, etc.

## Lista de Comandos básicos

* Ver la configuracion global de git.

    `git config --global --list`
* Cambiar el nombre de usuario en git

     ` git config --global user.name "<NOMBRE_USUARIO>"`

* Cambiar la direccion de correo

    ` git config --global user.email "<MAIL_USUARIO>"`

* Iniciar el Repositorio git

    `git init`

* Ver el estado del repositorio

    `git status`
* Adicionar archivos al repositorio

    ` git add <nobre_archivo>`

* Adicionar todos los archivos y carpetas

    ` git add -A ` ó ` git add .`

* Guardar archivos en el repositorio

    ` git commit -m " <mensaje_descriptivo_commit>"`

    -m: indaca que se agregara un mensaje al commmit, todo commit debe tener un mensaje que describa de forma general los cambios realizados.
* Ver el listado de commit realizados

    ` git log <numero_comit>`

* Ver  un commit realizado

    ` git log`

* Cambiar entre commit

    ` git checkout <numero_comit>`

* Ir al ultimo comit

    ` git checkout master`
* Borrar los comit

    ` git reset [--soft, --mixed, --hard ]` 

    --soft: Borra el commit pero no borra los archivos del disco.

    --mixed: No borra el Staging area ni el Working area

    --hard: Borra el commit y el archivo.

* Ver la ayuda de git

    ` git help [<comando>]`

## Ramas y fusiones

* Ver las ramas del repositorio

     `git branch`

* Crear Ramas

    `git branch <nombre_rama>`

    Notas: La rama se crea a partir de la rama y el commit en el que nos encontremos

* Pasar a una rama

    `git checkout <nombre_rama>`

* Fusionar una rama

    a - Pararse en la rama que reibira los cambio ` git checkout <rama_que_recibe>`
    
    b - fusionar las ramas `git merge <rama_que_contiene_los_cambios>`





