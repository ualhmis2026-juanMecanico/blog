# Introducción al Proyecto

**Fecha**: 14 de marzo de 2026  
**Autor**: [var500/Víctor Aguilar]

## Descripción del Proyecto
En este proyecto, nuestro equipo está desarrollando un blog estático utilizando Jekyll y desplegándolo en GitHub Pages y Azure. El objetivo es aprender sobre el desarrollo colaborativo, el uso de control de versiones con Git, y el despliegue de aplicaciones web, más concretamente en GitHub Pages.

## Objetivo
- Desplegar el blog en GitHub Pages.

## Pasos para el despliegue

### 1.- Ir a la configuración del repositorio
- Abrir el navegador y entrar a la página del repositorio en GitHub
- En el menú superior (donde dice Code, Issues, Pull requests...), haz clic en la última pestaña: Settings (Configuración).

### 2.- Entrar al menú de Pages
- En la barra lateral izquierda, desplazarnos hacia abajo hasta encontrar la sección Code and automation.
- Hacer clic en Pages.

### 3.- Elegir cómo se va a construir la página (Dos opciones)
- Opción A: Desplegar desde una rama (Deploy from a branch). Usarlo solo si se tiene una web estática simple (HTML/CSS), si se subió manualmente la carpeta final generada (public/ o _site/), o si se usa la integración básica de Jekyll que ofrece GitHub. Para realizarlo solamente hay que seleccionar Deploy from a branch. Luego, debajo en Branch, seleccionar tu rama main y la carpeta /root. Hacer clic en Save.

- Opción B: GitHub Actions (Recomendado para Hugo o Jekyll avanzado). Usarlo si se quiere que GitHub genere la página automáticamente cada vez que alguien hace un "merge" (acepta un Pull Request) usando el SSG. Para realizarlo, en el desplegable de Source, seleccionar GitHub Actions. GitHub detectará automáticamente qué se está usando (Jekyll o Hugo) y te sugerirá un flujo de trabajo. Hacer clic en Configure y luego en Commit changes para guardar ese archivo de configuración.

### 4.- Esperar a que se publique
- Una vez guardado (ya sea la Opción A o B), GitHub empezará a construir tu sitio. Se puede ver el progreso yendo a la pestaña Actions en el menú superior del repositorio.

- Cuando termine (suele tardar un par de minutos), si se vuelve a Settings > Pages, habrá un mensaje verde en la parte superior que dirá: "Your site is live at https://[tu-usuario].github.io/[nombre-del-repo]/"