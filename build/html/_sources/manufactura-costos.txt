************************
Manufactura - Costos
************************

Conceptos preliminares de costos
--------------------------------

.. toctree::
   :maxdepth: 2

   manufactura-costos-conceptos

Costos en Libertya
------------------

En Libertya los costos se organizan a partir de los siguientes elementos:
 
1. Elementos de Costos
2. Tipos de Costos
3. Costos de Producto
4. Costos indirectos


**Elementos de Costos**

Un Elemento de Costo, define la característica del costo de un producto:

	* Costo de Material: el costo se infiere del consumo de artículos.
	* Costo de Recurso: el costo se infiere del consumo de recursos.
	* Carga: el costo es cargado de forma manual.

1. Acceder a la ventana que se encuentra en el menú Costes → **Elemento de Coste**.
1. Acceder a la opción del menú **Costes → Elemento de Coste**. El sistema presenta una ventana como lo muestra la Imagen 57.
2. Campos a ingresar:

	* Compañía: Cliente para esta instalación compañía o entidad legal 
	* Organización: Entidad organizacional dentro de la compañía. Una organización es una unidad de la compañía o entidad legal.
	* Nombre: Identificador alfanumérico de la entidad. El nombre de una entidad (registro) se usa como una opción de búsqueda predeterminada adicional a la clave de búsqueda. El nombre es de hasta 60 caracteres de longitud.
	* Descripción: Descripción corta opcional del registro Una descripción esta limitada a 255 caracteres.
	* Activo: El registro está activo en el sistema Hay dos métodos para que los registros no estén disponibles en el sistema: Uno es eliminar el registro; el otro es desactivarlo. Un registro desactivado no está disponible para selección; pero está disponible para Informes.
	* Tipo de Elemento de Coste: define si el elemento para Materiales, Recursos, Carga.
	* Calculado: determina si de forma excluyente el Elemento es calculado por el sistema.
	* Predeterminado: determina si es el elemento por defecto.


.. figure:: _static/images/ly_elemcosto.png
    :alt: Elementos de Costos
    :align: center
    :figclass: align-center

    Imagen 57: Elementos de Costos


**Tipos de Costos**

Un Tipo de Costo, define el método de costeo de un producto:

	* Último Precio de Factura: obtiene e precio unitario, de la última factura del producto.
	* Promedio Facturación: obtiene e precio unitario, como un promedio de todas las facturas del producto.
	* Último Precio de Orden de Compra: obtiene e precio unitario, de la última orden de compra del producto.
	* Promedio de Orden de Compra: obtiene e precio unitario, como un promedio de todas las ordenes de compras del producto. 
	* Costo Estándar: obtiene e precio unitario, del precio configurado en la ventana Costes de Artículo en el campo Precio de Coste Actual.

1. Acceder a la opción del menú **Costes → Tipo de Coste**. El sistema presenta una ventana como lo muestra la Imagen 58.
2. Campos a ingresar:

	* Compañía: Cliente para esta instalación compañía o entidad legal 
	* Organización: Entidad organizacional dentro de la compañía. Una organización es una unidad de la compañía o entidad legal.
	* Nombre: Identificador alfanumérico de la entidad. El nombre de una entidad (registro) se usa como una opción de búsqueda predeterminada adicional a la clave de búsqueda. El nombre es de hasta 60 caracteres de longitud.
	* Ayuda: Mensaje corto opcional del registro de ayuda respecto de su significado.
	* Activo: El registro está activo en el sistema Hay dos métodos para que los registros no estén disponibles en el sistema: Uno es eliminar el registro; el otro es desactivarlo. Un registro desactivado no está disponible para selección; pero está disponible para Informes.
	* Método de Costeo: define la forma en la que se hace el cálculo de costo: Último Precio de Factura, Promedio Facturación, Último Precio de Orden de Compra, Promedio de Orden de Compra, Costo Estándar.


.. figure:: _static/images/ly_tipocosto.png
    :alt: Tipos de Costos
    :align: center
    :figclass: align-center

    Imagen 58: Tipos de Costos



**Costos de Producto**

Es la ventana que permite configurar una combinación de parámetros que definen el cálculo de costos para un producto.

1. Acceder a la opción del menú **Costes → Coste de Producto**. El sistema presenta una ventana como lo muestra la Imagen 59.
2. La primera pestaña, **Seleccionar Artículo** permite ubicar el artículo a configurar, es de solo lectura.
3. Para cargar los datos accedemos a la pestaña, **Costes de Artículo**. El sistema presenta una ventana como lo muestra la Imagen 60.
4. Campos a ingresar:

	* Compañía: Cliente para esta instalación compañía o entidad legal 
	* Organización: Entidad organizacional dentro de la compañía. Una organización es una unidad de la compañía o entidad legal.
	* Esquema Contable: Permite definir el Esquema Contable para la parametrización de costos.
	* Almacén: Permite definir el Almacén para la parametrización de costos.
	* Tipo de Coste: Permite definir el Tipo de Coste para la parametrización de costos.
	* Elemento de Coste: Permite definir el Elemento de Coste para la parametrización de costos.
	* Precio de Coste Actual: refleja el último costo calculado cuando corresponde o el costo ingresado manualmente para los casos de Costos Estándar.
	* Nota: el resto de los campos no aplican en la funcionalidad de esta versión.


.. figure:: _static/images/ly_costeart_1.png
    :alt: Artículo
    :align: center
    :figclass: align-center

    Imagen 59: Artículo

.. figure:: _static/images/ly_costeart_2.png
    :alt: Costes de Artículo
    :align: center
    :figclass: align-center

    Imagen 60: Costes de Artículo



**Asignación de Costos Manuales**

Este proceso, permite la asignación de costos manuales a la Orden de Manufactura. Su principal uso, está relacionado a la asignación de costos indirectos, pudiendo asignar los costos asociados a facturas de compra.

1. Acceder a la opción del menú **Costes → Asignar Costos Manuales**. El sistema presenta una ventana como lo muestra la Imagen 61.
2. Parámetros a ingresar:

	* **Esquema Contable:** Permite definir el Esquema Contable asociado a la asignación del costo manual. 
	* **Tipo de Costo:** Permite definir el Tipo de Costo asociado a la asignación del costo manual.
	* **Elemento de Costo:** Permite definir el Elemento de Costo asociado a la asignación del costo manual.
	* **Detalle de Costo:** Permite ingresar una leyenda de referencia.
	* **Orden de Manufactura:** Permite definir la Orden de Manufactura a la que se aplicará el costo.
	* Factura de Gastos: Permite definir una factura desde la que se tomará el monto de la aplicación del costo.
	* Valor del Costo: Permite definir de forma manual el monto de la aplicación del costo.


.. figure:: _static/images/ly_costemanual.png
    :alt: Asignación de Costos Manuales
    :align: center
    :figclass: align-center

    Imagen 61: Asignación de Costos Manuales



Ejemplo de configuración de costos
----------------------------------

.. toctree::
   :maxdepth: 2

   manufactura-costos-ejemplo

