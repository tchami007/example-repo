# Tutorial de Github
====================

1) Crear repositorio, por ejemplo example_repo

2) Crear el mismo directorio en la pc local

3) Clonar

git clone <nombre del repositorio>

Por ejemplo:

git clone https://github.com/tchami007/example-repo example_repo

4) Crear un archivo en la pc (local)

Por ejemplo:

readme.md

5) Solicitar el status

git status

Nota: Nos devuelve el estado del directorio local respecto del repositorio

6) Preparar el envio (stage)

git add <nombre del archivo>

Por ejemplo:

git add readme.md

NOTA: El archivo esta preparado, como si lo hubieramos puesto en una caja, pero aun no se ha enviado

7) Realizar el commit del envio (commit)

Por ejemplo:

git commit -m "Initial commit"

NOTA: El envio preparado ahora tiene un mensaje que es "Initial Commit". El mensaje es una etiqueta. Pero aun no se ha enviado.

8) Realizar el envio

Por ejemplo:

git push origin master

NOTA: Esta accion realiza el envio. Desde origin a la rama "master" del repositorio. Esto puede dar un error si la rama "master" no existe. Entonces:

git branch -m master

NOTA: Esta accion crea la rama "master" que faltaba en el punto anterior.



