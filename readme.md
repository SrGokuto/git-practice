# Comandos básicos de Git
`git clone <url_del_repositorio>`  Clona un repositorio remoto a tu máquina local.

`git init` Inicia un repositorio, Crea un nuevo repositorio Git en el directorio actual.

`git config` Configuraciones globales o especificas de un repositorio

`git add` Añade un archivo al área de preparación (staging area) para el commit 

`git commit` Establece el mensaje del commit

`git push` Envía los archivos del commit al repositorio

`git fetch` Trae información del repositorio (en caso de que se haya actualizado) pero no la combina con la información local

`git merge` Aplica los cambios detectados (en caso de existir) en `git fetch` a la rama local

## Gestión de cambios
`git status`  Muestra el estado actual del repositorio y los cambios pendientes.  

`git commit -m "Mensaje del commit"`  Crea un commit con los cambios agregados al área de preparación.

## Trabajando con ramas
`git branch`  Muestra las ramas existentes y la rama activa.

`git checkout <rama>`  Cambia a la rama especificada.  

`git merge <rama>`  Fusiona la rama especificada con la rama actual.

## Sincronización con repositorios remotos
`git push origin <rama>`  Envía los commits locales a la rama del repositorio remoto.  

`git pull origin <rama>`  Descarga y fusiona cambios del repositorio remoto a tu rama local.

## Configuración básica
`git config --global user.name "Tu Nombre"`  Establece el nombre de usuario en Git para todos los repositorios.

`git config --global user.email "tuemail@ejemplo.com"`  Establece el correo electrónico para Git.

### ¿Qué es un commit en Git?

`Un commit en GitHub` *es una instantánea de los cambios realizados en los archivos de un proyecto en un momento específico. Cuando se hace un commit, se guardan los cambios que se han preparado (con git add) en el repositorio local, creando una versión segura del proyecto que puede ser consultada o revertida posteriormente. Cada commit incluye un mensaje descriptivo que explica qué cambios se hicieron y tiene un identificador único (hash) que lo distingue de otros commits.*

-Es inmutable, lo que significa que una vez ha sido creado, no se puede modificar, aunque sí se puede deshacer con otros comandos.

-Tiene un identificador único, o hash, que lo diferencia de otros commits.

-También incluye un mensaje descriptivo, donde se explica qué cambios se realizaron.


### ¿Qué es un push en Git?

`Un push` *Es un comando de Git que transfiere y publica los cambios que has hecho en tu repositorio local a un repositorio remoto, como GitHub, GitLab o Bitbucket. Este comando sirve para actualizar la rama remota con las confirmaciones locales, permitiendo que otros miembros del equipo vean, revisen y colaboren en los mismos cambios.* 

-Publicación de cambios: Permite compartir tus commits locales con el resto del equipo, poniendo a disposición tus avances en un repositorio centralizado.

-Actualización de ramas: Por defecto, solo sube las commits de la rama que estás utilizando en el momento, pero puedes especificar a qué rama remota quieres enviar tus cambios usando la sintaxis git push <remoto> <branch>. 

-Envío masivo de ramas: Puedes subir todas las ramas de tu repositorio local al remoto utilizando la opción --all. 

-Subida de etiquetas: Permite enviar todas las nuevas etiquetas creadas localmente al repositorio remoto usando la opción --tags. 
# Proyecto de Prueba con Git

Este repositorio es un ejemplo para practicar los **comandos básicos de Git**.

## 🚀 Comandos principales

### Inicialización y configuración
- `git init` → Inicializa un repositorio en el directorio actual.
- `git config --global user.name "Tu Nombre"`
- `git config --global user.email "tuemail@ejemplo.com"`

### Gestión de cambios
- `git status` → Verifica el estado de los archivos.
- `git add archivo.txt` → Agrega un archivo específico.
- `git add .` → Agrega todos los archivos modificados.
- `git commit -m "mensaje"` → Crea un commit con mensaje.

### Sincronización
- `git push origin main` → Envía los commits al repositorio remoto.
- `git pull origin main` → Descarga y fusiona cambios del remoto.
# 📚 Guía Básica de Git

Este documento explica los comandos más comunes de Git y su uso en un flujo de trabajo real.


## 🔹 Flujo de trabajo típico
1. Clonar el repositorio:  
   `git clone <url>`

2. Crear una nueva rama para trabajar:  
   `git checkout -b nueva-rama`

3. Editar archivos y guardar cambios.

4. Añadir los archivos modificados:  
   `git add .`

5. Crear un commit con descripción:  
   `git commit -m "Implementada nueva funcionalidad X"`

6. Subir cambios al remoto:  
   `git push origin nueva-rama`

## 🔹 Ejemplo de comandos
- `git fetch` → Descarga referencias del remoto.
- `git merge <rama>` → Fusiona cambios en la rama actual.
- `git log --oneline` → Muestra el historial de commits resumido.
# 🛠️ Manual de Git para el equipo

Este repositorio incluye ejemplos y comandos de Git que utilizamos en el equipo de desarrollo.

## 📖 ¿Qué es Git?
Git es un sistema de control de versiones que permite trabajar en equipo, mantener un historial de cambios y colaborar en proyectos de software.

## 🔹 Configuración inicial
```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tucorreo@ejemplo.com"
# Crear una nueva rama
git branch feature/nueva-funcionalidad

# Cambiar a la rama creada
git checkout feature/nueva-funcionalidad

# Subir la nueva rama al remoto
git push -u origin feature/nueva-funcionalidad










