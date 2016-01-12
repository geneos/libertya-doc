*********************************
Manufactura - Lista de Materiales
*********************************

Lista de materiales
-------------------

Permite definir la composición de los productos fabricados, tanto intermedios como  terminados. Se pueden tener distintos niveles intermedios de producción, los  niveles intermedios definen la fabricación de productos que serán entrada de otros procesos productivos de niveles superiores.


Lista de materiales y fórmulas
------------------------------

1. Acceder a la ventana que se encuentra en el menú Gestión de Manufactura → Gestión de Ingeniería → Lista de Materiales y Fórmulas → **Lista de Materiales y Fórmula**.

2. Campos a ingresar en la cabecera:

* Compañía: Cliente para esta instalación compañía o entidad legal 
* Organización: Entidad organizacional dentro de la compañía. Una organización es una unidad de la compañía o entidad legal.
* Producto: Producto que va a tener una fórmula asociada.
* UM: Unidad de Medida se refiere a unidades de medida no monetarias y además define si se permite la conversión entre unidades de medida y cómo se van a calcular.
* Nombre: Identificador alfanumérico de la entidad. El nombre de una entidad (registro) se usa como una opción de búsqueda predeterminada adicional a la clave de búsqueda. El nombre es de hasta 60 caracteres de longitud. 
* Descripción: Descripción corta opcional del registro Una descripción esta limitada a 255 caracteres.
* Ayuda: El campo Ayuda contiene una sustento, comentario o ayuda acerca de cómo usar este item. 
* Activo: El registro está activo en el sistema Hay dos métodos para que los registros no estén disponibles en el sistema: Uno es eliminar el registro; el otro es desactivarlo. Un registro desactivado no está disponible para selección; pero está disponible para Informes 
* Aviso de Cambio Cuenta de materiales (ingeniería) cambio de aviso (versión).
* Nro del Documento: Número de secuencia del documento para cada documento creado. El número del documento es usualmente generado en automático por el sistema y determinado por el tipo del documento. Si el documento no se salva; el número preliminar se despliega entre "<>".
* Tipo LDM: Tipo de Lista de Materiales.
* LDM Usada: Uso de lista de materiales. El predeterminado de la LDM es usado, Si hay alternativos no están definidos.



3. Componentes de la LDM & Fórmula

Para cada componente se debe ingresar la siguiente información:

* No. Línea Indica el Número de Línea único y controlará el orden de despliegue de las líneas dentro de un documento.
* Artículo El Artículo en Lista de Materiales identifica un elemento/producto que es parte de una lista de materiales.
* Tipo de componente El tipo de componente debe ser alguno de los siguientes:
* Componente: identifica a una materia prima, ingrediente, parte o subproducto que es utilizado en el ensamblado de un proceso de fabricación superior.
    * Co producto: esta entidad no es un producto programado obtenido como consecuencia de otro proceso de producción. 
    * Empaque: este producto no será tenido en cuenta para calcular la cantidad total de componentes cuando la opción “Es Porcentaje Cantidad” se encuentre seleccionado.
    * Fantasma: indica que el producto es un ensamble ficticio, esto es, un conjunto de componentes que se agrupan sólo para hacer más fácil el análisis de forma separada del resto de la LDM. Cuando el MRP genera un requerimiento del fantasma y lo proyectado no está disponible, el proceso va al nivel mínimo y comienza un nuevo ciclo de MRP pero sin crear órdenes del producto fantasma.
    