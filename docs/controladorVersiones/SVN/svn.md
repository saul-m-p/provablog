---
sidebar_position: 1
---

# SVN

## interfaces graficas para git (GUI)

## TEORIA

- controlador de versiones centralizada;Centralizado vs. Distribuido: La principal diferencia entre SVN y Git radica en su arquitectura. SVN es un sistema de control de versiones centralizado, lo que significa que hay un único repositorio central que contiene la última versión del código y los desarrolladores trabajan directamente con este repositorio central. Git, por otro lado, es un sistema de control de versiones distribuido, lo que significa que cada desarrollador tiene una copia completa del repositorio, lo que les permite trabajar de forma independiente y fusionar sus cambios más tarde.

- Concepto de control de versiones: Al igual que Git, SVN es un sistema de control de versiones. Esto significa que te permite realizar un seguimiento de los cambios en tu código a lo largo del tiempo, facilitando la colaboración en proyectos y la gestión de cambios.

- Comandos básicos: Algunos de los comandos básicos en SVN son similares a los de Git, pero con diferentes nombres y sintaxis. Por ejemplo:

svn checkout es similar a git clone.
svn update es similar a git pull.
svn commit es similar a git commit.
svn status es similar a git status.

- Branches y etiquetas: En SVN, los conceptos de ramas (branches) y etiquetas (tags) son similares a los de Git, pero se gestionan de manera ligeramente diferente. En SVN, las ramas y etiquetas son directorios dentro del repositorio, mientras que en Git son punteros a instantáneas de un estado del repositorio.

- Historial de cambios: SVN y Git registran el historial de cambios de manera diferente. SVN utiliza un modelo de revisión incremental, donde cada revisión es un número entero secuencial. Git utiliza un modelo de gráfico acíclico dirigido (DAG), donde cada confirmación tiene un identificador único (SHA-1 hash) y se pueden fusionar ramas de manera más flexible.

- Integración con herramientas: Git es muy popular en la industria y tiene una amplia gama de herramientas y servicios que lo respaldan (como GitHub, GitLab, Bitbucket, etc.). SVN tiene menos herramientas modernas, pero aún se usa ampliamente en muchos proyectos de software.

### BUENAS PRACATICAS:

## COMANDOS

svnadmin create pathRepo - inicia repositorio.

svn checkout URL_del_repositorio: Clona un repositorio SVN en tu sistema local, descargando todos los archivos y directorios.

svn commit -m "Mensaje de confirmación descriptivo": Confirma los cambios realizados en tu copia de trabajo y los envía al repositorio con un mensaje descriptivo que explica los cambios realizados.

svn add nombre_del_archivo: Agrega archivos y directorios nuevos al control de versiones, preparándolos para ser confirmados en el próximo commit.

svn log: Muestra el historial de revisiones del repositorio, incluyendo información sobre cada revisión como el autor, la fecha y el mensaje de confirmación.

svn diff: Muestra las diferencias entre tu copia de trabajo y la revisión más reciente del repositorio, lo que te permite ver los cambios realizados.

svn revert nombre_del_archivo: Deshace los cambios locales en un archivo o directorio, restaurándolo a la última revisión del repositorio.

svn status: Muestra el estado de los archivos y directorios en tu copia de trabajo en relación con el repositorio, indicando si han sido modificados, agregados o eliminados.

svn info: Muestra información detallada sobre un archivo o directorio, incluyendo la URL del repositorio, la revisión actual y el autor.

svn copy origen destino: Copia archivos o directorios en el repositorio, creando una copia en el destino especificado.

svn delete nombre_del_archivo: Elimina archivos o directorios del control de versiones, marcándolos para ser eliminados en el próximo commit.

svn move origen destino: Mueve o renombra archivos o directorios en el repositorio, conservando el historial de versiones.

svn switch URL_del_repositorio: Cambia la URL del repositorio asociada con tu copia de trabajo, permitiéndote cambiar entre diferentes ramas o ubicaciones del repositorio.

svn merge URL_de_la_rama: Fusiona los cambios de una rama o revisión específica en tu copia de trabajo actual.

svn stash: Guarda temporalmente los cambios locales en una pila, permitiéndote trabajar en otra tarea y luego volver a aplicar los cambios guardados más tarde.

svn update: Actualiza tu copia local de trabajo con los cambios más recientes del repositorio.

svn tag nombre_de_la_etiqueta: Crea una etiqueta en el repositorio, marcando una revisión específica con un nombre significativo.

svn branch: Crea una nueva rama en el repositorio, permitiéndote trabajar en cambios separados del tronco principal.

svn list: Lista los archivos y directorios en un directorio del repositorio.

svn propset nombre_propiedad valor_propiedad nombre_del_archivo: Establece el valor de una propiedad específica en un archivo o directorio.

svn propget nombre_propiedad nombre_del_archivo: Obtiene el valor de una propiedad específica de un archivo o directorio.

svn propedit nombre_propiedad nombre_del_archivo: Edita el valor de una propiedad específica en un archivo o directorio.

svn propdel nombre_propiedad nombre_del_archivo: Elimina una propiedad específica de un archivo o directorio.

# estructura de svn (de la carpeta q crea)