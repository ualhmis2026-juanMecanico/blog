# Comandos Git

**Fecha**: 14 de marzo de 2026
**Autor**: [Sergio Alías García/sag854]

## Introducción
Git es un sistema de control de versiones distribuido y de código abierto que permite rastrear cambios en archivos, colaborar en proyectos de software de forma eficiente y gestionar diferentes versiones de un proyecto, facilitando el trabajo en equipo y la vuelta a estados anteriores si es necesario, sin depender de un servidor central para la mayoría de las operaciones.

## Configuración Inicial:
Antes de empezar, necesitamos hacer una configuración inicial:
* Configurar el nombre: `git config --global user.name "NOMBRE APELLIDOS"`
* Configurar tu email que será asociado a tus commits: `git config --global user.email "abc123@inlumine.ual.es"`

## Comandos utiles para git
### Iniciando repositorio
* Iniciamos GIT en la carpeta donde esta el proyecto: `git init`
* Clonamos el repositorio de GitHub: `git clone <url>`
* Añadimos todos los archivos para el commit: `git add .`
* Hacemos el primmer commit: `git commit -m "TEXTO"`
* Subimos al repositorio: `git push origin <rama>`

### Git add
* Añadimos todos los archivos para el commit: `git add .`
* Añadimos el archivo para el commit: `git add <archivo>`
* Añadimos todos los archivos para el commit omitiendo los nuevos: `git add --all`
* Añadimos todos los archivos con la extensión especificada: `git add *.txt`
* Añadimos todos los archivos dentro de un directorio y de una extensión especifica: `git add docs/*.txt`
* Añadimos todos los archivos dentro de un directorio: `git add docs/`

### Git commit
* Cargar en el HEAD los cambios realizados: `git commit -m "TEXTO"`
* Agregar al ultimo commit, se puede especificar un nuevo mensaje: `git commit --amend -m "TEXTO"`

### Git push
* Subimos al repositorio: `git push <origen> <branch>`
* Subimos un tag: `git push --tags`

## Git head
* Saca un archivo del commit: `git reset HEAD <archivo>`
* Devuelve el ultimo commit que se hizo y pone los cambios en staging: `git reset --soft HEAD^`

## Git branch
* Crea un branch: `git branch <nameBranch>`
