***************
Módulo de Stock
***************

**Datos previos necesarios**


1. Almacenes y Ubicaciones
2. Artículos
3. Conjunto de Atributos (Opcional)
4. Cargos


Proceso de gestión de stock
---------------------------


1. Ingresos de Artículos al Stock
	A. Ingresos por **Remito de Compras** (Ver módulo de Compras).
	B. Ingresos por ajuste de **Inventario Físico**.
	C. Ingresos por **Remito de Devolución de Clientes** (Ver módulo de Ventas). 
	D. Ingresos por **Devolución de Materiales para Producción**  (Ver módulo de Producción).
	E. Cambio de Artículo.


2. Movimientos de Stock entre Almacenes
	A. **Movimiento de Inventario**.
	B. **Transferencia de Mercadería**.
		1. **Transferencia en dos Etapas**.
		2. **Movimiento en dos Etapas**. Por ejemplo para envíos a garantía.
	C. **Entradas y Salidas Simples**. Por ejemplo para pérdidas.

3. Bajas de Stock
	A. Baja por ajuste de **Inventario Físico**.
	B. Baja por **Entrega de Materiales para Producción** (Ver módulo de Producción).
	C. Baja lógica por Movimientos de Inventario a almacenes de descarte.
	D. Baja por **Remito de Entrega a Clientes** (Ver módulo de Compras).
	E. Baja por **Remito de Devolución a Proveedores** (Ver módulo de Ventas).
	F. Cambio de Artículo.


Almacenes y Ubicaciones
-----------------------

Para poder almacenar artículos y tenerlos disponibles como stock, primero se han de definir una serie de Almacenes o Ubicaciones donde se almacenaran dichos productos.

**Almacén**

Para esto se utiliza la ventana de Almacén. En la pestaña principal se introduce un nombre y una dirección física para nuestro almacén, a fin de que dicha dirección pueda constar en los documentos que se generen. Este último dato es obligatorio.

1. Acceder a la opción de menú **Entidades Configuración de la Compañía → Almacén y Ubicaciones**, por defecto ingresa a la primera pestaña de **Almacén**, el sistema presenta una ventana como lo muestra la Imagen 22.
2. Campos a ingresar:
	* Compañía
	* Organización
	* Clave de Búsqueda
	* Nombre
	* Descripción
	* Activo
	* Localización / Dirección
	* Cargo de Fraccionamiento
	* Cargo de Merma
	* Cargo x Cambio de Artículo 

.. figure:: _static/images/ly_alm1.png
    :alt: Almacenes
    :align: center
    :figclass: align-center

    Imagen 22: Almacenes

**Ubicación**

En la siguiente pestaña se define cada una de las ubicaciones de las que costara el almacén.

Una ubicación es una combinación de un pasillo, una estantería y un nivel de profundidad. Esto permite definir todas las combinaciones de almacenamiento posibles. Adicionalmente, se puede definir una prioridad para que los artículos salgan primero de una determinada ubicación.

1. Acceder a la pestaña **Ubicación**, el sistema presenta una ventana como lo muestra la Imagen 23.
2. Campos a ingresar:
	* Compañía
	* Organización
	* Almacén
	* Clave de Búsqueda
	* Activo
	* Prioridad Relativa
	* Predeterminado
	* Pasillo (X)
	* Estanteria (Y)
	* Nivel (Z) 

.. figure:: _static/images/ly_alm2.png
    :alt: Ubicaciones
    :align: center
    :figclass: align-center

    Imagen 23: Ubicaciones

**Almacenamiento**

En la tercera pestaña se podrá consultar a posteriori que artículos ha sido  asignados a la ubicación que se hubieran seleccionado en la pestaña anterior.

1. Acceder a la pestaña **Almacenamiento**, el sistema presenta una ventana como lo muestra la Imagen 24.
2. Campos que informa la pestaña:
	* Compañía
	* Organización
	* Ubicación
	* Artículo
	* Instancia del Conjunto de Attributos
	* Activo
	* Stock
	* Ultima Fecha de Recuento de Inventarios
	* P. Servir
	* P. Recibir 

.. figure:: _static/images/ly_alm3.png
    :alt: Almacenamiento
    :align: center
    :figclass: align-center

    Imagen 24: Almacenamiento


Cargos
------

Para algunas de las operaciones con Stock, se deben configurar elementos especiales, para detallar motivos y/o hacer afectación contable. Para esto se utilizan los **Cargos**.

1. Acceder a la opción de menú **Contabilidad → Configuración de Contabilidad → Cargo**, por defecto ingresa a la primera pestaña de **Almacén**, el sistema presenta una ventana como lo muestra la Imagen 25.
2. Campos que informa la pestaña:
	* Compañía
	* Organización
	* Clave de Búsqueda
	* Nombre
	* Descripción
	* Activo
	* Tipo de Cargo
	* Signo
	* Importe de Cargo
	* Categoría del Impuesto
	* Impuesto Incluido en el Precio
	* Mismo Impuesto  
3. Acceder a la pestaña **Contabilidad**, el sistema presenta una ventana como lo muestra la Imagen 26.
4. Campos que informa la pestaña:
	* Compañía
	* Organización
	* Cargo
	* Esquema Contable
	* Activo
	* Cuenta de Otros Gastos
	* Cuenta de Otros Ingresos  


.. figure:: _static/images/ly_cargo.png
    :alt: Cargo
    :align: center
    :figclass: align-center

    Imagen 25: Cargo

.. figure:: _static/images/ly_cargo_cont.png
    :alt: Contabilidad de Cargo
    :align: center
    :figclass: align-center

    Imagen 26: Contabilidad de Cargo

 

Inventario Físico
-----------------

Esta ventana se utiliza para realizar ajustes manuales al Stock.

1. Acceder a la opción de menú **Almacén → Inventario Físico**, por defecto ingresa a la primera pestaña de **Recuento de Inventario**, el sistema presenta una ventana como lo muestra la Imagen 27.
2. Campos que informa la pestaña:
	* Compañía
	* Organización
	* Nro. Del Documento
	* Descripción
	* Tipo de Documento
	* Fecha de Movimiento
	* Almacén
	* Configuracion de Inventario
	* Generar Lista
	* Actualizar Cantidades
	* Proyecto
	* Campaña
	* Aprobación
	* Cantidad Aprobada
	* Estado del Documento
	* Acción en el Documento
3. Acceder a la pestaña **Línea de Recuento de Inventario**, el sistema presenta una ventana como lo muestra la Imagen 28.
4. Campos que informa la pestaña:
	* Compañía
	* Organización
	* Inventario Físico
	* Nro. Línea
	* Descripción
	* Artículo
	* Ubicación
	* Cantidad Contada
	* Cantidad según el sistema
	* Diferencia
	* Tipo de Inventario
	* Cargo (en caso que el Tipo de Inventario sea Cargo en Cuenta)


.. figure:: _static/images/ly_invfisico_1.png
    :alt: Inventario Físico
    :align: center
    :figclass: align-center

    Imagen 27: Inventario Físico

.. figure:: _static/images/ly_invfisico_2.png
    :alt: Inventario Físico - Líneas
    :align: center
    :figclass: align-center

    Imagen 28: Inventario Físico - Líneas


Movimientos de Inventario
-------------------------

Esta ventana se utiliza para realizar transferencias entre almacenes.

1. Acceder a la opción de menú **Almacén → Movimiento de Inventario**, por defecto ingresa a la primera pestaña de **Movimiento**, el sistema presenta una ventana como lo muestra la Imagen 29.
2. Campos que informa la pestaña:
	* Compañía
	* Organización
	* Nro. Del Documento
	* Descripción
	* Fecha de Movimiento
	* Tipo de Documento
	* Proyecto
	* Campaña
	* Aprobación
	* Cantidad Aprobada
	* En Tránsito
	* Fecha de Recibo
	* Estado del Documento
	* Acción en el Documento
3. Acceder a la pestaña **Línea de Movimiento**, el sistema presenta una ventana como lo muestra la Imagen 30.
4. Campos que informa la pestaña:
	* Compañía
	* Organización
	* Movimiento
	* Nro. Línea
	* Descripción
	* Activo
	* Artículo
	* Conj. Atributos Origen
	* Conj. Atributos Destino
	* Ubicación
	* A Ubicación
	* Cantidad del Movimiento
	* Cantidad Destino
	* Cantidad Desechada
	* Cantidad Confirmada


.. figure:: _static/images/ly_mov_1.png
    :alt: Movimiento de Inventario
    :align: center
    :figclass: align-center

    Imagen 29: Movimiento de Inventario

.. figure:: _static/images/ly_mov_2.png
    :alt: Movimiento de Inventario - Líneas
    :align: center
    :figclass: align-center

    Imagen 30: Movimiento de Inventario - Líneas


**Transferencia de Mercadería**

**Entradas y Salidas Simples**

