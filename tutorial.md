# Tutorial de Github


En este tutorial, vamos a explicar los comandos basicos para manejar el repositorio Github desde la linea de comandos. Consideramos aprender desde la lina de comandos como primera etapa, ya que siempre nos enfrentaremos a la posiblidad de tener que correr estos comandos manuales. Además asegurar una mejor compresion del tema.

## Conceptos Previos
### Instalación de Github en nuestro PC
Antes de comenzar, es necesario comenzar con la instalacion de GitHub en nuestro PC. Para ello, dependiendo del SO, vamos a recurrir a una version u otra. Para la descarga de la version en windows, usaremos:

Luego, instalamos el componente en nuestra pc.

### Repositorio
El repositorio, es una ubicacion "en la nube" donde se va colocar el codigo de nuestra aplicación. La aplicación puede ser cierto código en texto plano. 
### Local
La carpeta o directorio del equipo o pc desde donde vamos a desarrollar nuestro codigo de la aplicación.

La idea es "mantener" sincronizados ambas ubicaciones: local y repositorio. Los comandos que vamos a ver en esta etapa comenzarán con una carpeta local en nuestro pc, la cual vamos a "vincular" a un repositorio de github que previmanete vamos a crear.
## Comencemos...
1) Crear repositorio, por ejemplo "example_repo"

El primer paso será la creacion de un repositorio dentro de GitHub. Para ello, primero accedemos a una cuenta de Github (o la creamos si no la disponemos aun). Dentro de la pantalla principal, ubicamos en el sector superior derecho el botón "+" (new repository). En ese punto nos va a solicitar el nombre del repositorio, y una descripción sintetica de su contenido. Tambien nos va a solicitar otras características mas: 
- radio button Publico o Privado (vamos a usar publico, ya que privado es pago)
- checkbox para readme file (vamos a dejarlo sin chequear)
- add .gitignore (no lo usamos ahora)
- choose license (no lo usamos ahora)
Finalmente, le damos al boton verde "Create repository"

2) Crear el mismo directorio en la pc local

Luego, nos vamos a nuestro PC y nos ubicamos dentro de un directorio que vamos a usar como "local". Dentro de ese directorio (que debe estar vacio), dejamos nuestro prompt del SO, listo para ingresar nuestros comandos de GitHub.

3) Clonar el repositorio
`git clone <nombre del repositorio> <Nombre de Carpeta(opcional)>`
Por ejemplo:
`git clone https://github.com/tchami007/example-repo example_repo`

NOTA: La clonacion, crea un vinculo entre el directorio LOCAL y el REPOSITORIO. Este vinculo queda registrado para seguimiento (tracking) en GitHub.  En la sintaxis, se puede ver un nombre de carpeta, en este caso se uso "example_repo". Cuando termina de correrse este primer comando, se habra creado una carpeta llamada "example_repo" dentro del directorio donde estabamos. Esa carpeta sera la que estará sincronizada para seguimiento. Para finalizar este paso, nos moveremos dentro de esta carpeta.

4) Crear un archivo en la pc (local)
Por ejemplo:
`readme.md`

5) Solicitar el status
`git status`
Nota: Nos devuelve el estado del directorio local respecto del repositorio

6) Preparar el envio (stage)
`git add <nombre del archivo>`
Por ejemplo:
`git add readme.md`

NOTA: El archivo esta preparado, como si lo hubieramos puesto en una caja, pero aun no se ha enviado

7) Realizar el commit del envio (commit)
Por ejemplo:
`git commit -m "Initial commit"`

NOTA: El envio preparado ahora tiene un mensaje que es "Initial Commit". El mensaje es una etiqueta. Pero aun no se ha enviado.

8) Realizar el envio
Por ejemplo:
`git push origin master`

NOTA: Esta accion realiza el envio. Desde origin a la rama "master" del repositorio. Esto puede dar un error si la rama "master" no existe. Entonces:
`git branch -m master`

NOTA: Esta accion crea la rama "master" que faltaba en el punto anterior.
