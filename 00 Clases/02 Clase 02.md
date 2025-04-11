# Introducción a Git y GitHub

## Repaso a Git

Git es un sistema de control de versiones distribuido. Permite llevar un registro de los cambios en el código fuente a lo largo del tiempo. Es ampliamente utilizado en el desarrollo de software para colaborar entre múltiples desarrolladores y mantener un historial de cambios.
- Distribuido: Cada desarrollador tiene una copia completa del repositorio en su máquina local.
- Historial: Permite ver el historial de cambios, revertir a versiones anteriores y comparar diferentes versiones del código.
- Integridad de datos: Utiliza un sistema de hash (SHA-1) para asegurar la integridad de los datos.


### Funcionamiento de Git

- Area de trabajo: Donde se realizan los cambios en los archivos.
- Area de preparación (staging area): Donde se preparan los cambios antes de hacer un commit.
- Repositorio local: Donde se almacenan los commits y el historial de cambios.

### Que son los commits

Un commit es una instantánea del estado del proyecto en un momento dado. Cada commit tiene un identificador único (hash) y puede incluir un mensaje descriptivo que explique los cambios realizados. Los commits permiten llevar un registro de la evolución del proyecto y facilitan la colaboración entre desarrolladores.

- Es la unidad fundamental de trabajo en Git.
- Podemos verlo como un snapshot del proyecto en un momento dado.


## Comandos básicos de Git

- `git init`: Inicializa un nuevo repositorio Git en el directorio actual.
- `git clone <url>`: Clona un repositorio remoto en el directorio local.
- `git add <archivo>` `git add .` `git add A` `git add --all`: Agrega un archivo al área de preparación.
- `git commit -m "<mensaje>"`: Realiza un commit de los cambios en el área de preparación.
- `git status`: Muestra el estado del repositorio (archivos modificados, archivos en el área de preparación, etc.).
- `git log`: Muestra el historial de commits.
- `git diff`: Muestra las diferencias entre los archivos modificados y el último commit.
- `git branch`: Muestra las ramas del repositorio.
- `git checkout <rama>`: Cambia a la rama especificada.
- `git merge <rama>`: Fusiona la rama especificada con la rama actual.
- `git pull`: Actualiza el repositorio local con los cambios del repositorio remoto.
- `git push`: Envía los cambios locales al repositorio remoto.
- `git remote add <nombre> <url>`: Agrega un repositorio remoto.
- `git remote -v`: Muestra los repositorios remotos configurados.
- `git fetch`: Descarga los cambios del repositorio remoto sin fusionarlos.
- `git reset <archivo>`: Deshace los cambios en el área de preparación.
- `git reset --hard`: Deshace todos los cambios en el área de trabajo y el área de preparación.
- `git stash`: Guarda los cambios no confirmados en un área temporal. como en una pila, se puede revertir a un commit anterior y luego volver a aplicar los cambios guardados en el stash.
- `git stash pop`: Recupera los cambios guardados en el stash.
- `git cherry-pick <commit>`: Aplica un commit específico a la rama actual.
- `git rebase <rama>`: Reaplica los commits de la rama actual sobre la rama especificada.
- `git tag <nombre>`: Crea una etiqueta (tag) en el commit actual.
- `git show <tag>`: Muestra información sobre una etiqueta específica.
- `git reflog`: Muestra el historial de referencias (reflog) del repositorio.
- `git bisect`: Ayuda a encontrar un commit que introdujo un error en el código.
- `git blame <archivo>`: Muestra quién modificó cada línea de un archivo.
- `git config --global user.name "<nombre>"`: Configura el nombre de usuario para los commits.
- `git config --global user.email "<email>"`: Configura el correo electrónico para los commits.
- `git config --global core.editor "<editor>"`: Configura el editor de texto predeterminado para Git.
- `git config --global color.ui auto`: Habilita el color en la salida de Git.
- `git config --global alias.<alias> <comando>`: Crea un alias para un comando de Git.
- `git config --list`: Muestra la configuración actual de Git.
- `git help <comando>`: Muestra la ayuda para un comando específico de Git.
- `git help -a`: Muestra una lista de todos los comandos disponibles en Git.
- `git help -g`: Muestra una lista de las guías de uso de Git.
- `git help -s`: Muestra una lista de los comandos más comunes de Git.
- `git help -p`: Muestra una lista de los comandos más comunes de Git con ejemplos.
- `git help -e`: Abre la ayuda de Git en el editor de texto configurado.
- `git help -w`: Abre la ayuda de Git en el navegador web.
- `git show <commit>`: Muestra información detallada sobre un commit específico.
- `git checkout <commit>`: Cambia a un commit específico.
- `git reset <commit>`: Deshace los cambios hasta un commit específico.

### GitFlow

GitFlow es un modelo de ramificación para Git que define un conjunto de reglas y convenciones para gestionar el desarrollo de software. Se basa en la idea de tener ramas específicas para diferentes propósitos, como desarrollo, producción y características nuevas.

- `master`: Rama principal que contiene la versión estable del proyecto.
- `develop`: Rama de desarrollo donde se integran las nuevas características.
- `feature/<nombre>`: Rama para desarrollar una nueva característica.
- `release/<nombre>`: Rama para preparar una nueva versión del proyecto.
- `hotfix/<nombre>`: Rama para corregir errores críticos en producción.
- `support/<nombre>`: Rama para soporte de versiones anteriores del proyecto.
- `bugfix/<nombre>`: Rama para corregir errores en el desarrollo.
- `experiment/<nombre>`: Rama para experimentar con nuevas ideas o tecnologías.
- `chore/<nombre>`: Rama para tareas de mantenimiento o limpieza del código.
- `refactor/<nombre>`: Rama para refactorizar el código sin cambiar su funcionalidad.
- `test/<nombre>`: Rama para pruebas y validaciones del código.
- `docs/<nombre>`: Rama para documentación del proyecto.
- `style/<nombre>`: Rama para cambios de estilo y formato del código.
- `perf/<nombre>`: Rama para mejorar el rendimiento del código.
- `ci/<nombre>`: Rama para integración continua y automatización de pruebas.
- `ops/<nombre>`: Rama para operaciones y despliegue del proyecto.
- `ux/<nombre>`: Rama para mejoras en la experiencia de usuario.
- `ui/<nombre>`: Rama para mejoras en la interfaz de usuario.
- `api/<nombre>`: Rama para cambios en la API del proyecto.
- `db/<nombre>`: Rama para cambios en la base de datos del proyecto.
- `config/<nombre>`: Rama para cambios en la configuración del proyecto.
- `build/<nombre>`: Rama para cambios en el proceso de construcción del proyecto.
- `deploy/<nombre>`: Rama para cambios en el proceso de despliegue del proyecto.

Recomendación minima:

- `main`: Rama principal que contiene la versión estable del proyecto.
- `develop`: Rama de desarrollo donde se integran las nuevas características.
- `staging`: Rama de pruebas antes de la producción.

Buena práctica en uso de prefijos:

- `feature/`: Rama para desarrollar una nueva característica.
- `bugfix/`: Rama para corregir errores en el desarrollo.
- `hotfix/`: Rama para corregir errores críticos en producción.
- `release/`: Rama para preparar una nueva versión del proyecto.
- `experiment/`: Rama para experimentar con nuevas ideas o tecnologías.
- `chore/`: Rama para tareas de mantenimiento o limpieza del código.
- `refactor/`: Rama para refactorizar el código sin cambiar su funcionalidad.
- `test/`: Rama para pruebas y validaciones del código.
- `docs/`: Rama para documentación del proyecto.
- `style/`: Rama para cambios de estilo y formato del código.
- `perf/`: Rama para mejorar el rendimiento del código.
- `ci/`: Rama para integración continua y automatización de pruebas.
- `ops/`: Rama para operaciones y despliegue del proyecto.
- `ux/`: Rama para mejoras en la experiencia de usuario.
- `ui/`: Rama para mejoras en la interfaz de usuario.
- `api/`: Rama para cambios en la API del proyecto.
- `db/`: Rama para cambios en la base de datos del proyecto.
- `config/`: Rama para cambios en la configuración del proyecto.
- `build/`: Rama para cambios en el proceso de construcción del proyecto.
- `deploy/`: Rama para cambios en el proceso de despliegue del proyecto.


## Gitignore

El archivo `.gitignore` se utiliza para especificar qué archivos o directorios deben ser ignorados por Git. Esto es útil para evitar que archivos temporales, de configuración local o de compilación sean incluidos en el repositorio.

## Nuevo Repositorio
## Commit
## Ramas