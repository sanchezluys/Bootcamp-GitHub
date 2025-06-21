# Repositorios

Instructor: Luis Beltrán

## Que son los repositorios

Un repositorio es un espacio de almacenamiento donde se guarda el código fuente de un proyecto, junto con su historial de cambios. Los repositorios permiten a los desarrolladores colaborar, gestionar versiones y mantener un registro de las modificaciones realizadas en el código.

- Puede ser
  - Público: Accesible para cualquier persona, ideal para proyectos de código abierto.
  - Privado: Accesible solo para usuarios autorizados, adecuado para proyectos privados o confidenciales.
  - Interno: Accesible solo para miembros de una organización, útil para proyectos internos de empresas.

### Ramas o branchs

Las ramas son versiones paralelas del código dentro de un repositorio. Permiten a los desarrolladores trabajar en diferentes características o correcciones sin afectar la rama principal (generalmente llamada "main" o "master"). Las ramas facilitan la colaboración y el desarrollo simultáneo de múltiples funcionalidades.

### Clonar

Clonar un repositorio significa crear una copia local del mismo en tu máquina. Esto te permite trabajar en el código sin necesidad de estar conectado a Internet. Al clonar un repositorio, obtienes todo el historial de cambios y las ramas disponibles.

### Fork

Un fork es una copia de un repositorio que permite a los desarrolladores realizar cambios sin afectar al repositorio original. Es útil para contribuir a proyectos de código abierto, ya que permite experimentar y proponer mejoras sin comprometer el código principal.

### Merge

El merge es el proceso de combinar los cambios realizados en una rama con otra. Por lo general, se utiliza para integrar características desarrolladas en ramas separadas a la rama principal del proyecto. El merge puede generar conflictos si los cambios realizados en ambas ramas afectan las mismas líneas de código, lo que requiere una resolución manual.

### Pull Request

Un pull request es una solicitud para fusionar cambios realizados en una rama a otra. Permite revisar y discutir los cambios antes de integrarlos al código principal. Los pull requests son una herramienta clave para la colaboración en proyectos de código abierto, ya que facilitan la revisión del código y la discusión entre los colaboradores.

### Remoto

Un repositorio remoto es una versión del repositorio que se aloja en un servidor, como GitHub, GitLab o Bitbucket. Los repositorios remotos permiten a los desarrolladores colaborar y compartir código con otros usuarios a través de Internet. Puedes clonar un repositorio remoto para trabajar localmente y luego enviar tus cambios al repositorio remoto mediante comandos de Git.

### Upstream

El upstream se refiere al repositorio original del cual se ha hecho un fork o clon. Es importante mantener una conexión con el upstream para poder recibir actualizaciones y cambios realizados por los desarrolladores originales. Esto permite sincronizar tu fork o clon con las últimas modificaciones del proyecto.

### Downstream

El downstream se refiere a los repositorios que han sido creados a partir de un fork o clon del repositorio original. Los desarrolladores que trabajan en un downstream pueden realizar cambios y mejoras, pero deben estar atentos a las actualizaciones del upstream para mantener su código actualizado.

### Roles

#### Roles en una organización

1. Read: Permite a los usuarios ver el contenido del repositorio, pero no realizar cambios. Ideal para colaboradores que solo necesitan consultar el código.
2. Write: Permite a los usuarios realizar cambios en el repositorio, como agregar o modificar archivos. Es adecuado para colaboradores activos que contribuyen al desarrollo del proyecto.
3. Triage: Permite a los usuarios gestionar issues y pull requests, asignar tareas y realizar un seguimiento del progreso del proyecto. Es útil para coordinadores o líderes de equipo.
4. Maintain: Permite a los usuarios gestionar el repositorio, incluyendo la configuración, la administración de ramas y la gestión de colaboradores. Es adecuado para administradores del proyecto.
5. Admin: Permite a los usuarios tener control total sobre el repositorio, incluyendo la capacidad de eliminarlo, cambiar su visibilidad y gestionar la configuración de seguridad. Es el rol más alto y debe ser asignado con precaución.

### Seguridad del repositorio

1. Dependabot: Es una herramienta que ayuda a mantener las dependencias del proyecto actualizadas y seguras. Analiza las dependencias del repositorio y sugiere actualizaciones para corregir vulnerabilidades conocidas.
2. Secret scanning: Es una característica que busca automáticamente secretos y credenciales sensibles en el código del repositorio. Ayuda a prevenir filtraciones de información confidencial y a mantener la seguridad del proyecto.
3. Code scanning: Es una herramienta que analiza el código en busca de vulnerabilidades y problemas de seguridad. Proporciona informes detallados sobre posibles riesgos y sugiere soluciones para mejorar la seguridad del código.

## Archivos Readme y buenas practicas, y archivos especiales

Un archivo README es un documento que proporciona información sobre el proyecto, incluyendo su propósito, cómo instalarlo, cómo usarlo y cualquier otra información relevante. Es una buena práctica incluir un README en cada repositorio para facilitar la comprensión del proyecto a otros desarrolladores.
Usa marckdown.

- Es lo primero que se ve al entrar a un repositorio.
- Atrae colaboradores.
- Establece expectativas.
- Proporciona instrucciones.
- Presenta características.
- Genera confianza.

Buenas prácticas para un README:

1. **Título y descripción**: Comienza con un título claro y una breve descripción del proyecto. una imagen, banner o logo del proyecto.
2. **Tabla de contenidos**: Incluye una tabla de contenidos para facilitar la navegación por el README, especialmente si es extenso.
3. **Instalación**: Proporciona instrucciones claras sobre cómo instalar y configurar el proyecto. Incluye requisitos previos, comandos de instalación y cualquier configuración adicional necesaria.
4. **Uso**: Explica cómo utilizar el proyecto, incluyendo ejemplos de comandos o código. Si es una aplicación, proporciona capturas de pantalla o GIFs para ilustrar su funcionamiento.
5. **Contribución**: Incluye pautas para contribuir al proyecto, como cómo enviar pull requests, reportar problemas o participar en discusiones. Esto fomenta la colaboración y ayuda a mantener un estándar de calidad en el código.
6. **Licencia**: Especifica la licencia bajo la cual se distribuye el proyecto. Esto es importante para que los usuarios comprendan sus derechos y restricciones al utilizar el código.
7. **Contacto**: Proporciona información de contacto para que los usuarios puedan comunicarse contigo en caso de dudas o problemas. Esto puede incluir tu correo electrónico, perfil de GitHub o enlaces a redes sociales.
8. Añade un badge de estado del proyecto, como el estado de construcción, cobertura de pruebas o número de descargas. Esto proporciona información rápida sobre la salud del proyecto y su actividad.

### Archivos especiales

- Readme: Un archivo README es un documento que proporciona información sobre el proyecto, incluyendo su propósito, cómo instalarlo, cómo usarlo y cualquier otra información relevante. Es una buena práctica incluir un README en cada repositorio para facilitar la comprensión del proyecto a otros desarrolladores.
- Contributing: Un archivo CONTRIBUTING.md es un documento que describe cómo los colaboradores pueden contribuir al proyecto. Incluye pautas para enviar pull requests, reportar problemas y participar en discusiones. Es útil para establecer expectativas claras y fomentar la colaboración.
- License: Un archivo LICENSE es un documento que especifica la licencia bajo la cual se distribuye el código del repositorio. Es importante elegir una licencia adecuada para proteger tus derechos y los de los usuarios. Existen diferentes tipos de licencias, como la MIT, GPL, Apache, entre otras.
- Code of Conduct: Un archivo CODE_OF_CONDUCT.md es un documento que establece las normas de comportamiento esperadas de los colaboradores del proyecto. Fomenta un ambiente inclusivo y respetuoso, y proporciona pautas para manejar situaciones de acoso o discriminación.
- Codeowners: Un archivo CODEOWNERS es un documento que define quiénes son los responsables de revisar y aprobar cambios en el código del repositorio. Es útil para asignar responsabilidades y garantizar que los cambios sean revisados por las personas adecuadas antes de ser fusionados.
- security: Un archivo SECURITY.md es un documento que proporciona información sobre cómo reportar vulnerabilidades de seguridad en el proyecto. Incluye pautas para informar sobre problemas de seguridad y cómo se manejarán las divulgaciones responsables.

Hay mas archivos.

## Manejo de repositorios creación y visibilidad

- Si se cambia la visibilidad se pierden las estrellas y forks.

## Añadir archivos a un repositorio

- Los archivos se pueden añadir a un repositorio utilizando la interfaz web de GitHub o mediante comandos de Git en la terminal.

## Manejo de cambios de un repositorio

- Los cambios en un repositorio se gestionan mediante commits, que son instantáneas del estado del código en un momento dado. Cada commit debe tener un mensaje descriptivo que explique los cambios realizados.
- Los commits se pueden realizar utilizando la interfaz web de GitHub o mediante comandos de Git en la terminal.

## Clonar un repositorio

- Clonar un repositorio significa crear una copia local del mismo en tu máquina. Esto te permite trabajar en el código sin necesidad de estar conectado a Internet.

## Crear Ramas

- Las ramas son versiones paralelas del código que permiten trabajar en diferentes características o correcciones sin afectar la rama principal (generalmente llamada "main" o "master").

## Estrellas y otras características sociales de un repositorio

- Las estrellas son una forma de mostrar aprecio por un repositorio y pueden ser utilizadas para marcar proyectos interesantes.

## Menu de un repositorio

### Wikis

- Los wikis son secciones dentro de un repositorio donde se puede documentar el proyecto de manera más detallada. Permiten a los colaboradores agregar y editar contenido fácilmente.

### Forks

- Un fork es una copia de un repositorio que permite a los desarrolladores realizar cambios sin afectar al repositorio original. Es útil para contribuir a proyectos de código abierto.

### Licencias

- Las licencias son documentos legales que especifican cómo se puede utilizar, modificar y distribuir el código de un repositorio. Es importante elegir una licencia adecuada para tu proyecto para proteger tus derechos y los de los usuarios.
- Existen diferentes tipos de licencias, como la MIT, GPL, Apache, entre otras. Cada una tiene sus propias condiciones y restricciones.

### Issues

- Los issues son una forma de rastrear errores, características solicitadas o cualquier otra tarea relacionada con el proyecto. Permiten a los colaboradores discutir y gestionar el trabajo pendiente.

### Pull Requests

- Los pull requests son solicitudes para fusionar cambios realizados en una rama a otra. Permiten revisar y discutir los cambios antes de integrarlos al código principal.

### Discusiones

- Las discusiones son una forma de comunicación dentro de un repositorio donde los colaboradores pueden plantear preguntas, compartir ideas o discutir sobre el proyecto. Es una herramienta útil para fomentar la colaboración y la comunidad en torno al proyecto.

### Actions

- GitHub Actions es una herramienta de integración continua y entrega continua (CI/CD) que permite automatizar flujos de trabajo dentro de un repositorio. Puedes configurar acciones para compilar, probar y desplegar tu código automáticamente cuando se realicen cambios en el repositorio.

### Projects

- Los proyectos son una forma de organizar y gestionar el trabajo dentro de un repositorio. Permiten crear tableros Kanban, asignar tareas y realizar un seguimiento del progreso del proyecto.

### Seguridad

- La seguridad en un repositorio implica proteger el código y los datos sensibles, así como gestionar los permisos de acceso de los colaboradores. Es importante revisar regularmente las configuraciones de seguridad y aplicar buenas prácticas para evitar vulnerabilidades.

### Insights

- Los insights proporcionan estadísticas y métricas sobre el repositorio, como el número de contribuciones, la actividad de los colaboradores y el uso de las ramas. Estas métricas pueden ayudar a comprender mejor el estado del proyecto y la participación de la comunidad.

### Gist

- Los gists son una forma de compartir fragmentos de código o notas de manera rápida y sencilla. Son útiles para compartir ejemplos de código, configuraciones o cualquier otro contenido que no requiera un repositorio completo.
- Secret Gists: Son gists privados que solo pueden ser vistos por el creador y las personas a las que se les comparta el enlace. Son útiles para compartir información sensible o confidencial sin hacerla pública.
- Public Gists: Son gists públicos que pueden ser vistos por cualquier persona. Son útiles para compartir código o información que se desea hacer accesible a la comunidad.
- Se puede clonar o forkear un gist, lo que permite trabajar en él de manera similar a un repositorio normal. También se pueden crear issues y pull requests en gists, lo que facilita la colaboración y el seguimiento de cambios.

### Feed

- El feed es una sección donde se muestra la actividad reciente del repositorio, incluyendo commits, pull requests, issues y otras acciones realizadas por los colaboradores. Permite mantenerse actualizado sobre los cambios y el progreso del proyecto.

## GitHub Pages

- GitHub Pages es una característica que permite alojar sitios web estáticos directamente desde un repositorio de GitHub. Es útil para crear documentación, blogs o páginas de proyectos sin necesidad de configurar un servidor web.
- Para crear un sitio web con GitHub Pages, se debe crear una rama llamada "gh-pages" o utilizar la rama principal del repositorio. Luego, se pueden agregar archivos HTML, CSS y JavaScript para construir el sitio.
- GitHub Pages también permite utilizar generadores de sitios estáticos como Jekyll, Hugo o Gatsby para crear sitios web más complejos y personalizados. Estos generadores facilitan la creación de contenido dinámico y la gestión de plantillas.
