*******************************
Manufactura - Flujos de Trabajo
*******************************

**Definir el flujo de trabajo de manufactura y la lista de recursos utilizados en producción**

Antes de dar de alta nuevos recursos de manufactura, debemos generar los **Tipos de Recurso.**

Los **Tipo de recurso de manufactura** proveen un agrupamiento mediante una relación jerárquica: por ejemplo un **centro de trabajo** se puede integrar en una **estación de trabajo, una línea de producción**, que a su vez junto a otras líneas se integran en una **Planta**. Esta agrupación de tipos de recursos, se utilizará para calcular la capacidad requerida y disponible de producción mediante la sumatoria individual de las capacidades de cada recurso.

Un primer nivel de agrupamiento será utilizado para definir una tipología de recursos que tengan en común una serie de características.

Definición de Tipos de Recursos
*******************************

Ir a Gestión de Ingenieria, Recursos de Manufactura, Tipo de Recurso de Manufactura y hacer click en el icono de nuevo registro  para generar un tipo de recurso.

* **Compañía** Cliente para esta instalación Compañía ó entidad legal 
* **Organización** Entidad organizacional dentro de la compañía.
* **Clave de Búsqueda** Clave de búsqueda para el registro en el formato requerido; debe ser única.
* **Nombre** Identificador alfanumérico de la entidad. El nombre de una entidad (registro) se usa como una opción de búsqueda predeterminada adicional a la clave de búsqueda. El nombre es de hasta 60 caracteres de longitud. 
* **Descripción** Descripción corta opcional del registro Una descripción esta limitada a 255 caracteres.
* **Activo** El registro está activo en el sistema Hay dos métodos para que los registros no estén disponibles en el sistema: Uno es eliminar el registro; el otro es desactivarlo. Un registro desactivado no está disponible para selección; pero está disponible para Informes. 
* **UM** Unidad de Medida La UM define una unidad de medida única (dias, horas, kilos, litros).
* **Permitir fracciones de UM** Permitir fracciones de unidad de medida Si se habilita; se puede entrar fracciones de la unidad de medida. 
* **Categoría del Producto** Categoría de la que este producto es parte Identifica la categoría a la que pertenecen este producto. 
* **Categoría del Impuesto** La categoría de impuesto proporciona un método de agrupación de impuestos similares. 
* **Asignación Única solamente** Solamente una asignación a la vez (No se puede tener asignaciones dobles de tiempo o asignaciones concurrentes) Si se selecciona; solo se puede tener una asignación a la vez para un momento en el tiempo. No es posible tener asignaciones concurrentes.
* **Tiempo Disponible** Indica si el recurso tiene tiempo disponible Indica si el recurso está disponible sólo en algún momento
* **Inicio** Momento cuando el tiempo disponible comienza Momento cuando el tiempo disponible comienza
* **Final** Momento cuando el tiempo disponible finaliza Momento cuando el tiempo disponible termina
* **Día Disponible** Recurso tiene disponibilidad del día Recurso solo esta disponible algunos días (lunes, martes...)


Recurso de manufactura
----------------------

Ahora podemos definir todos los Recursos de Manufactura, clasificados mediante los tipos de recursos, para poder utilizarlos luego en el flujo de trabajo.

Un **Recurso de Manufactura** es cualquier cosa requerida como soporte para el proceso de producción. Principalmente responde a la pregunta: ¿En dónde se hace un producto?. Cada recurso de trabajo es único dentro de la organización y puedo definir tantos recursos como sea necesario.

Definición de Recursos
----------------------

Ir a Gestión de Ingenieria, Recursos de Manufactura, Recurso de Manufactura y hacer click en el icono de nuevo registro  para generar un nuevo recurso.

* **Compañía** Cliente para esta instalación Compañía ó entidad legal 
* **Organización** Entidad organizacional dentro de la compañía Una organización es una unidad de la compañía o entidad legal 
* **Clave de Búsqueda** Clave de búsqueda para el registro en el formato requerido; debe ser única Una clave de búsqueda le permite a usted un método rápido de encontrar un registro en particular 
* **Nombre** Identificador alfanumérico de la entidad. El nombre de una entidad (registro) se usa como una opción de búsqueda predeterminada adicional a la clave de búsqueda. El nombre es de hasta 60 caracteres de longitud. 
* **Descripción** Descripción corta opcional del registro Una descripción está limitada a 255 caracteres.
* **Activo** El registro está activo en el sistema Hay dos métodos para que los registros no estén disponibles en el sistema: Uno es eliminar el registro; el otro es desactivarlo. Un registro desactivado no está disponible para selección; pero está disponible para Informes.
* **Tipo de Recurso** Es el tipo de recurso Manufactura registrado en el paso anterior.  
* **Almacén** El Almacén indica un Almacén único donde los productos son almacenados.  
* **Usuario** Indica un usuario de referencia o contacto.
* **Disponible** Indica si el recurso está disponible.
* **Es Recurso Manufactura** Indica si el recurso es requerido para la producción
* **Tiempo Encolado** Es una referencia donde se ingresa el tiempo total de encolado del recurso.
* **Tiempo de espera** El tiempo de preparación es el requerido para ejecutar las actividades necesarias para preparar el recurso de manufactura hasta que esté listo para comenzar con el proceso de fabricación.