#####################################
Gestión del Proyecto de Documentación
#####################################

Para el mantenimiento de la documentación se va a trabajar con una combinación de tecnologías que incluyen:

	- Sphinx: es una herramienta que permite escribir documentos en texto plano, formato rst, para una fácil generación de salidas en formatos que satisfagan diversas necesidades, en nuestro caso usaremos salida a html. La documentación de texto plano también es útil para colaboradores a través de distintos sistemas. El texto plano es uno de los formatos más portables disponibles actualmente. Se puede pensar en Sphinx como una infraestructura de documentación que abstrae las partes tediosas y ofrece funcionalidad automática para solucionar problemas comunes como el indexado de títulos y el resaltado de código especial.
	- Git: para realizar el seguimiento de los cambios y la salida de versiones. Usaremos para esto la infraestructura de Github, donde se alojará el repositorio.


Metodología de trabajo con Git
------------------------------

Como introducción a Git, recomendamos la lectura y la ejercitación a partir de   `Git-La Guía Sencilla <http://rogerdudler.github.io/git-guide>`_. 

**Obtener el código de la documentación**

Para esto ejecutamos el siguiente comando en el directorio donde queremos tener el proyecto::

	git clone git@github.com:geneos/libertya-doc.git

**Trabajar con los archivos del proyecto**

Me muevo al branch de desarrollo actual con git checkout (por ejemplo trabajamos diferentes sprint o iteraciones, para incorporar cambios y modificaciones por temas)::

	git checkout sprint-1

Creó un nuevo branch a partir de este antes de comenzar el desarrollo (por ejemplo trabajamos con un branck por requerimiento). Este branch puede permanecer de manera local o se puede subir si es necesario, ejemplo::

	git checkout -b REQ-1

Estoy creando un nuevo branch en el que voy a incorporar la información del   REQ-1.

Se comienza a trabajar sobre los archivos de documentación, se puede:

	- Modificar un archivo existente.
	- Agregar nuevos archivos.
	- Reorganizar los archivos existentes.

Si necesito compartir lo que realizamos con algún miembro del equipo, o quiero tener el trabajo en un repositorio remoto se puede subir el branch usando::

	# Agregamos cada archivo modificado o creado
	git add ruta_archivo
	# Confirmamos el conjunto de archivos agregados
	git commit -m "Mensaje que resuma la naturaleza de los cambios"
	# Si queremos subir los commit a un repositorio remoto
	git push origin REQ-1

Nota: En lo posible es preferible solo un commit por requerimiento, pero si es necesario se pueden hacer varios commits, solo complica un poco el trabajo del git master ante un problema en la integración.

Ahora es necesario actualizar el nodo actual REQ-1 con cualquier posible cambio que se haya subido al branch sprint-1 (Esto puede o no ser necesario, para esto es necesaria la comunicación entre los colaboradores). Esto se hace de la siguiente manera::

	git pull --rebase

Básicamente lo que realiza es actualizar nuestro nodo base, al estado del branch que le digamos, en este caso sprint-1 y luego ubica todos los commits nuestros por encima, de forma que es como si hubiéramos arrancado a desarrollar desde el estado actual de sprint-1.

Durante dicha operación pueden surgir conflictos (Porque existen modificaciones en las mismas líneas de los mismos archivos realizadas por otros colaboradores), en este caso se notificara por pantalla qué archivos están en conflicto y el desarrollador debe revisarlos y hacer un merge manual de dichos archivos y una vez corregidos hacer::

	git add ruta_archivo
	git rebase --continue 

Una vez completado nuestro branch está listo para ser mergeado al branch del sprint-1.

Nos movemos al branch de desarrollo actual con git checkout::

	git checkout sprint-1

Hacemos un merge con nuestros desarrollos::

	git merge REQ-1
	
En este punto no debería existir ningún conflicto, ya que previamente nos aseguramos de que todos nuestros cambios sean nodos posteriores al estado actual.

Una vez finalizado entonces si se hace git push del branch desarrollo y se notifica a los demás desarrolladores::

	git push origin sprint-1

Es decisión de los demás desarrolladores si hacer un rebase en ese momento de sus branches locales en los que están desarrollando los requerimientos para quedar al mismo nivel que el branch de desarrollo o si lo hacen antes de integrarlo con el branch de desarrollo.

Para comenzar un nuevo desarrollo entonces se procede de la misma manera, creando un nuevo branch a partir de el branch de desarrollo.

Es potestad del Git Master integrar los desarrollos de los colaboradores en la versión base desde la que se liberan versiones generales.

Si bien el Git Master es uno de los colaboradores, proponemos que sea ejecutor de las acciones planificadas por un equipo de coordinación seleccionado por el conjunto de los colaboradores.

Renderizar a HTML con Sphinx
----------------------------

Una vez que tenemos el proyecto y queremos validar como se va estructurando la documentación, hacemos uso del render a html de Sphinx. Para esto en la carpeta del proyecto, ejecutamos::

	make html

Esto crea una carpeta con los archivos en ruta_proyecto/build/html/

