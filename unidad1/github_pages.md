# Acerca de GitHub Pages
GitHub Pages es un servicio de alojamiento de sitio estático que toma archivos HTML, CSS y JavaScript directamente desde un repositorio en GitHub, opcionalmente ejecuta los archivos a través de un proceso de complilación y publica un sitio web. Puede ver ejemplos de sitios de GitHub Pages en la colección de ejemplos de GitHub Pages.

Puede hospedar el sitio en el dominio github.io de GitHub o un dominio personalizado propio. 

## Tipos de sitios GitHub Pages
Existen tres tipos básicos de GitHub Pages sitios: de **proyecto**, de **usuario** y de la **organización**. Los sitios de proyecto están conectados con un proyecto específico alojado en GitHub. Los sitios de usuario y de organización se conectan a una cuenta específica en GitHub.com.

Para publicar un sitio de usuario, debes crear un repositorio propiedad de la cuenta personal denominado `username.github.io`. 

Para publicar un sitio de organización, debe crear un repositorio propiedad de una organización denominado `organization.github.io`.

A menos que use un dominio personalizado, los sitios de usuario y organización están disponibles en http(s)://userna.github.io o http(s)://<organization>.github.io.
Los archivos fuente para un sitio de proyecto se almacenan en el mismo repositorio que su proyecto. A menos que use un dominio personalizado, los sitios de proyecto están disponibles en http(s)://<username>.github.io/<repository> o http(s)://<organization>.github.io/<repository>.
Solo puedes crear un sitio de organización o de usuario para cada cuenta en GitHub. Los sitios de proyectos, ya sean propiedad de una cuenta de organización o personal, son ilimitados.

Publicar fuentes para sitios de GitHub Pages
Puedes publicar el sitio cuando se inserten cambios en una rama específica o puedes escribir un flujo de trabajo de GitHub Actions para publicar el sitio.

Si no necesitas ningún control sobre el proceso de creación del sitio, se recomienda publicar el sitio cuando se inserten cambios en una rama específica. Puedes especificar qué rama y carpeta usar como origen de publicación. La rama de origen puede ser cualquier rama del repositorio y la carpeta de origen puede ser la raíz del repositorio (/) de la rama de origen o una carpeta /docs de la rama de origen. Cuando se insertan cambios en la rama de origen, los cambios en la carpeta de origen se publicarán en el sitio de GitHub Pages.


Generadores de sitios estáticos
GitHub Pages publica cualquier archivo estático que subas a tu repositorio. Puedes crear tus propios archivos estáticos o usar un generador de sitios estáticos para que desarrolle tu sitio. 
También puedes personalizar tu propio proceso de compilación de forma local o en otro servidor.

Si usas un proceso de compilación personalizado o un generador de sitios estáticos distinto de Jekyll, puedes escribir un GitHub Actions para compilar y publicar el sitio. 
GitHub proporciona flujos de trabajo de inicio para varios generadores de sitios estáticos. 

Si publicas el sitio desde una rama de origen, GitHub Pages usará Jekyll para compilar tu sitio de forma predeterminada. 
Si quieres usar un generador de sitios estáticos distinto de Jekyll, se recomienda escribir un GitHub Actions para compilar y publicar tu sitio en su lugar. De lo contrario, desactiva el proceso de compilación de Jekyll creando un archivo vacío denominado .nojekyll en la raíz de la fuente de publicación y, después, sigue las instrucciones del generador de sitios estáticos para crear el sitio localmente.

GitHub Pages no soporta idiomas del lado del servidor como PHP, Ruby o Python.

****************************************************

Crear un sitio de Páginas de GitHub
Crear un repositorio para tu sitio
Puedes crear un repositorio o elegir un repositorio existente para el sitio.

Si quieres crear un sitio de GitHub Pages para un repositorio donde no todos los archivos del repositorio están relacionados con el sitio, podrás configurar una fuente de publicación para el sitio. 
Por ejemplo, puedes tener una rama dedicada y una carpeta para contener los archivos de origen del sitio , o bien usar un flujo de trabajo de GitHub Actions personalizado para compilar e implementar los archivos de origen del sitio.

Si la cuenta a la que pertenece el repositorio utiliza GitHub Free o GitHub Free para organizaciones, el repositorio deberá ser público.

Si quiere crear un sitio en un repositorio existente, vaya a la sección "Crear tu sitio".
En la esquina superior derecha de cualquier página, utiliza el menú desplegable  y selecciona New repository (Nuevo repositorio).

Captura de pantalla del menú desplegable GitHub que muestra las opciones para crear nuevos elementos. El elemento de menú "New repository" está resaltado en naranja oscuro.

Usa el menú desplegable Propietario para seleccionar la cuenta que quieres que sea propietaria del repositorio.
Captura de pantalla del menú del propietario de un repositorio de GitHub nuevo. El menú muestra dos opciones, octocat y github.

Escribe un nombre para tu repositorio y una descripción opcional. Si va a crear un sitio de usuario u organización, el repositorio debe tener el nombre <user>.github.io o <organization>.github.io. Si tu nombre de organización o usuario contiene mayúsculas, debes hacerlas minúsculas. Para obtener más información, vea «Acerca de GitHub Pages».
Captura de pantalla de la configuración de GitHub Pages en un repositorio. El campo del nombre del repositorio contiene el texto "octocat.github.io" y aparece en naranja oscuro.

Elige la visibilidad del repositorio. Para obtener más información, vea «Acerca de los repositorios».

Seleccione Initialize this repository with a README (Inicializar este repositorio con un archivo Léame).

Haga clic en Create repository (Crear repositorio).

Crear tu sitio
Antes de que puedas crear tu sitio, debes tener un repositorio para el mismo en GitHub. Si no va a crear el sitio en un repositorio existente, vea "Creación de un repositorio para el sitio".

Advertencia: Los sitios de GitHub Pages están disponibles públicamente en Internet, incluso si el repositorio del sitio es privado. Si tienes datos confidenciales en el repositorio del sitio, tal vez te interese eliminarlos antes de publicarlo. Para obtener más información, vea «Acerca de los repositorios».

En GitHub, navega al repositorio de tu sitio.

Decide qué fuente de publicación quieres utilizar. Para obtener más información, vea «Configurar una fuente de publicación para tu sitio de Páginas de GitHub».

Crea el archivo de entrada para el sitio. GitHub Pages buscará un archivo index.html, index.md o README.md como archivo de entrada para el sitio.

Si el origen de publicación es una rama y una carpeta, el archivo de entrada debe estar en el nivel superior de la carpeta de origen de la rama de origen. Por ejemplo, si la fuente de publicación es la carpeta /docs de la rama main, el archivo de entrada debe estar en la carpeta /docs de una rama denominada main.

Si la fuente de publicación es un flujo de trabajo de GitHub Actions, el artefacto que implementes debe incluir el archivo de entrada en el nivel superior del artefacto. En lugar de agregar el archivo de entrada al repositorio, puedes optar por que el flujo de trabajo de GitHub Actions genere el archivo de entrada cuando se ejecute el flujo de trabajo.

Configura tu fuente de publicción. Para obtener más información, vea «Configurar una fuente de publicación para tu sitio de Páginas de GitHub».

En el nombre del repositorio, haz clic en  Configuración. Si no puedes ver la pestaña "Configuración", selecciona el menú desplegable  y, a continuación, haz clic en Configuración.
Captura de pantalla de un encabezado de repositorio en el que se muestran las pestañas. La pestaña "Configuración" está resaltada con un contorno naranja oscuro.

En la sección "Código y automatización" de la barra lateral, haz clic en  Páginas.

Para ver el sitio publicado, en "GitHub Pages", haz clic en  Visitar sitio.
Captura de pantalla de un mensaje de confirmación para GitHub Pages que muestra la dirección URL del sitio. A la derecha de la dirección URL, aparece un botón con la etiqueta "Visitar sitio" en color naranja oscuro.

Nota: Es posible que la publicación de los cambios en el sitio tome hasta 10 minutos después de que envíes los cambios a GitHub. Si no ves los cambios del sitio de GitHub Pages reflejados en el explorador después de una hora, consulta "Acerca de los errores de compilación para sitios de Páginas de GitHub".

Su GitHub Pages sitio se construye y se implementa con un GitHub Actions flujo de trabajo. Para más información, consulta "Visualizar el historial de ejecución del flujo de trabajo".

Nota GitHub Actions es gratuito para los repositorios públicos. Los cargos de uso se aplican a repositorios privados e internos que van más allá de la asignación mensual de minutos gratuitos. Para más información, consulta "Límites de uso, facturación y administración".

Notas:

Si publicas desde una rama y el sitio no se ha publicado automáticamente, asegúrate de que alguien con permisos de administrador y una dirección de correo electrónico verificada haya insertado en la fuente de publicación.

Las confirmaciones insertadas por un flujo de trabajo de GitHub Actions que usa GITHUB_TOKEN no desencadenan una compilación de GitHub Pages.

Pasos siguientes
Puedes agregar más páginas a tu sitio creando más archivos nuevos. Cada archivo estará disponible en tu sitio en la misma estructura de directorios que tu fuente de publicación. Por ejemplo, si el origen de publicación del sitio del proyecto es la rama gh-pages y crea un nuevo archivo denominado /about/contact-us.md en la rama gh-pages, el archivo estará disponible en https://<user>.github.io/<repository>/about/contact-us.html.

También puedes agregar un tema para personalizar la apariencia de tu sitio. Para más información, consulta "Agregar un tema a tu sitio de Páginas de GitHub con Jekyll".

Para personalizar aún más tu sitio, puedes usar Jekyll, un generador de sitio estático con soporte integrado para GitHub Pages. Para más información, consulta "Acerca de las Páginas de GitHub y Jekyll".

Información adicional
"Solucionar problemas de errores de compilación de Jekyll para sitios de Páginas de GitHub"
"Crear y eliminar ramas en tu repositorio"
"Crear nuevos archivos"
"Solución de errores 404 en sitios de GitHub Pages"
Ayuda y soporte técnico
