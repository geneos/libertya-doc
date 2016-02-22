*******************************
Manufactura - Flujos de Trabajo
*******************************

Los Flujos de Trabajo de Manufactura, definen la estructura de **Etapas productivas** y **Recursos** asociados a cada etapa.

Tipos de Recursos de Manufactura
--------------------------------

Los **Tipo de Recurso de Manufactura** proveen un agrupamiento mediante una relación jerárquica: por ejemplo un **Centro de Trabajo** se puede integrar en una **Estación de Trabajo**, una **Línea de Producción**, que a su vez junto a otras líneas se integran en una **Planta**. Esta agrupación de tipos de recursos, se utilizará para calcular la capacidad requerida y disponible de producción mediante la sumatoria individual de las capacidades de cada recurso.

Un primer nivel de agrupamiento será utilizado para definir una tipología de recursos que tengan en común una serie de características.

1. Acceder a la opción del menú **Gestión de Ingeniería →  Recursos de Manufactura → Tipo de Recurso de Manufactura**. El sistema presenta una ventana como lo muestra la Imagen 32.
2. Campos a ingresar:
	* **Compañía:** Cliente para esta instalación Compañía o entidad legal 
	* **Organización:** Entidad organizacional dentro de la compañía.
	* **Clave de Búsqueda** Clave de búsqueda para el registro en el formato requerido; debe ser única.
	* **Nombre:** Identificador alfanumérico de la entidad. El nombre de una entidad (registro) se usa como una opción de búsqueda predeterminada adicional a la clave de búsqueda. El nombre es de hasta 60 caracteres de longitud. 
	* **Descripción:** Descripción corta opcional del registro Una descripción esta limitada a 255 caracteres.
	* **Activo:** El registro está activo en el sistema Hay dos métodos para que los registros no estén disponibles en el sistema: Uno es eliminar el registro; el otro es desactivarlo. Un registro desactivado no está disponible para selección; pero está disponible para Informes. 
	* **UM:** Unidad de Medida La UM define una unidad de medida única (días, horas, kilos, litros).
	* **Permitir fracciones de UM:** Permitir fracciones de unidad de medida Si se habilita; se puede entrar fracciones de la unidad de medida. 
	* **Asignación Única solamente:** Solamente una asignación a la vez (No se puede tener asignaciones dobles de tiempo o asignaciones concurrentes) Si se selecciona; solo se puede tener una asignación a la vez para un momento en el tiempo. No es posible tener asignaciones concurrentes.
	* **Tiempo Disponible:** Indica si el recurso está disponible sólo en algún momento, habilita los campos Inicio y Final.
	* **Inicio:** Momento cuando el tiempo disponible comienza.
	* **Final:** Momento cuando el tiempo disponible finaliza.
	* **Día Disponible:** Indica si el recurso está disponible sólo algunos días de la semana, habilita los campos para cada uno de los días (lunes, martes, miércoles, jueves, viernes, sábado y domingo).
3. Guardar.

.. figure:: _static/images/ly_tiporecurso.png
    :alt: Tipo de Recurso de Manufactura
    :align: center
    :figclass: align-center

    Imagen 32: Tipo de Recurso de Manufactura


Recurso de manufactura
----------------------

Ahora podemos definir todos los Recursos de Manufactura, clasificados mediante los Tipos de Recursos, para poder utilizarlos luego en el Flujo de Trabajo.

Un **Recurso de Manufactura** es cualquier cosa requerida como soporte para el proceso de producción. Principalmente responde a la pregunta: ¿En dónde se hace un producto?. Cada recurso de trabajo es único dentro de la organización y puedo definir tantos recursos como sea necesario.

1. Acceder a la opción del menú **Gestión de Ingeniería →  Recursos de Manufactura → Recurso de Manufactura**. El sistema presenta una ventana como lo muestra la Imagen 33.
2. Campos a ingresar:
	* **Compañía:** Cliente para esta instalación Compañía o entidad legal 
	* **Organización:** Entidad organizacional dentro de la compañía.
	* **Tipo de Recurso: ** Es el Tipo de Recurso de Manufactura registrado en el paso anterior.	
	* **Clave de Búsqueda** Clave de búsqueda para el registro en el formato requerido; debe ser única.
	* **Nombre:** Identificador alfanumérico de la entidad. El nombre de una entidad (registro) se usa como una opción de búsqueda predeterminada adicional a la clave de búsqueda. El nombre es de hasta 60 caracteres de longitud. 
	* **Descripción:** Descripción corta opcional del registro Una descripción esta limitada a 255 caracteres.
	* **Activo:** El registro está activo en el sistema Hay dos métodos para que los registros no estén disponibles en el sistema: Uno es eliminar el registro; el otro es desactivarlo. Un registro desactivado no está disponible para selección; pero está disponible para Informes. 
	* **Almacén:** El Almacén indica un Almacén único donde los productos son almacenados.  
	* **Usuario:** Indica un usuario de referencia o contacto.
	* **Disponible:** Indica si el recurso está disponible.
	* **Es Recurso Manufactura:** Indica si el recurso es requerido para la producción. Este campo debe estar seleccionado.
	* **Tipo de Recurso Manufactura:** Es el Tipo de Recurso Manufactura General, al menos uno de los Recursos debe ser del tipo **Planta** y deberá configurarse en el Flujo de Trabajo de Manufactura. 
	* **Tiempo Encolado:** Es una referencia donde se ingresa el tiempo total de encolado del recurso.
	* **Tiempo de espera:** El tiempo de preparación es el requerido para ejecutar las actividades necesarias para preparar el recurso de manufactura hasta que esté listo para comenzar con el proceso de fabricación.
3. Guardar.


.. figure:: _static/images/ly_recurso.png
    :alt: Recurso de Manufactura
    :align: center
    :figclass: align-center

    Imagen 33: Recurso de Manufactura
