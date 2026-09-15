# Creación y sincronización de repositorios con Git y GitHub

**Nombre:** Vanessa Mariana Hernandez Moreno
**Matrícula:** 2530411

## Objetivo

Que el estudiante sea capaz de crear y administrar un repositorio local en Git, utilizar el *Staging Area*, realizar *commits*, vincular un repositorio local con GitHub y sincronizar cambios utilizando `git push` y `git pull`.

## Descripción del procedimiento realizado

1. Crear una carpeta para el proyecto.
2. Abrir PowerShell y entrar a la carpeta creada.
3. Inicializar el repositorio local utilizando los comandos adecuados de Git.
4. Crear dos archivos:

   * `datos.txt`
   * `README.md`
5. Verificar el estado del repositorio.
6. Agregar los archivos al *Staging Area*.
7. Crear un *commit* para guardar los cambios.
8. Crear un repositorio vacío en GitHub.
9. Vincular el repositorio local con el repositorio remoto de GitHub mediante su URL.
10. Verificar que el repositorio local y el repositorio de GitHub estén correctamente vinculados.
11. Realizar un cambio desde GitHub y utilizar `git pull` para comprobar que el cambio aparezca en la computadora.
12. Realizar un cambio desde el repositorio local.
13. Verificar el estado del repositorio.
14. Realizar un *commit* y utilizar `git push` para enviar la modificación a GitHub.
15. Comprobar nuevamente que la modificación se haya realizado correctamente.

## Comandos de Git utilizados

* `git add`
* `git status`
* `git init`
* `git commit -m "nombre"`
* `git remote -v`
* `git push -u origin main`
* `git pull origin main`
* `git push`
* `git branch -m main`

## Explicación breve de la función de cada comando

### `git add`

Agrega los cambios de los archivos a la zona de preparación (*Staging Area*) antes de realizar un *commit*. Por ejemplo, `git add .` agrega todos los cambios.

### `git status`

Muestra el estado actual del repositorio, incluyendo archivos modificados, nuevos o pendientes de agregar.

### `git init`

Inicializa una carpeta como un repositorio local de Git.

### `git commit -m "nombre"`

Guarda los cambios preparados en el historial de Git mediante un mensaje que describe la modificación realizada.

### `git remote -v`

Muestra las conexiones o URLs de los repositorios remotos, como el repositorio de GitHub.

### `git push -u origin main`

Sube los cambios de la rama `main` del repositorio local a GitHub y establece `origin/main` como referencia para futuros comandos `push` y `pull`.

### `git pull origin main`

Descarga los cambios de la rama `main` desde GitHub y los integra en el repositorio local.

### `git push`

Sube los *commits* realizados localmente al repositorio remoto configurado, normalmente GitHub.

### `git branch -m main`

Cambia el nombre de la rama actual a `main`.

## ¿Cómo se creó el repositorio local?

Para crear el repositorio local primero se creó una carpeta para el proyecto. Después se abrió PowerShell y se ingresó a dicha carpeta utilizando el comando `cd`.

Una vez dentro de la carpeta, se ejecutó:

```bash
git init
```

Este comando inicializó la carpeta como un repositorio local de Git.

## ¿Cómo se vinculó el repositorio local con GitHub?

Primero se ingresó al repositorio local y se inicializó Git. Después se cambió el nombre de la rama principal a `main`:

```bash
git branch -m main
```

Posteriormente, se vinculó el repositorio local con el repositorio remoto de GitHub utilizando su URL:

```bash
git remote add origin URL_DEL_REPOSITORIO
```

Finalmente, se comprobó que la vinculación se hubiera realizado correctamente utilizando:

```bash
git remote -v
```

## Sincronización Local → GitHub

La sincronización de **Local → GitHub** consiste en enviar los cambios realizados en la computadora al repositorio remoto de GitHub.

El proceso básico es:

```bash
git add .
git commit -m "Descripción de los cambios"
git push
```

Primero se preparan los archivos con `git add`, después se guardan los cambios en el historial mediante `git commit` y finalmente se envían a GitHub utilizando `git push`.

## Sincronización GitHub → Local

La sincronización de **GitHub → Local** consiste en descargar los cambios que existen en el repositorio de GitHub y actualizar el repositorio que se encuentra en la computadora.

Para realizarlo se utiliza:

```bash
git pull origin main
```

Este comando descarga los cambios de GitHub y los integra en el repositorio local.

## Descripción de los archivos contenidos en el repositorio

### `datos.txt`

Contiene una explicación básica del ejercicio y se utiliza para realizar y comprobar actualizaciones mediante *commits* y sincronización.

### `README.md`

Contiene los pasos realizados, la descripción del ejercicio, el nombre del alumno, la matrícula y otra información general importante sobre el proyecto.

## Conclusión personal sobre lo aprendido

Como conclusión, aprendí a utilizar comandos básicos de Git y a sincronizar repositorios locales de la computadora con repositorios remotos en GitHub. También comprendí la importancia de comprobar varias veces que los cambios se hayan realizado correctamente.

Además, reforcé mis conocimientos sobre Markdown y obtuve una idea más amplia de cómo gestionar código, controlar versiones y trabajar con repositorios durante el desarrollo de proyectos.
