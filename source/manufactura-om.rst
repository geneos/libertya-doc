**********************************
Manufactura - Orden de Manufactura
**********************************

<<<<<<< HEAD
Una Orden de Manufactura es un documento que indica a la planta el compromiso de
fabricar un producto en una cantidad establecida y en una fecha específica.
Para  generar  o  modificar  manualmente  una  Orden  de  Manufactura  debemos ir a:
Manufactura -> Control de Producción -> Manufactura Discreta -> Orden de Manufactura.

La Orden de Manufactura integra componentes de la lista de materiales, del flujo de
trabajo y de los datos de planeamiento.

**Fecha de última Entrega**:Es la fecha de la última vez que el material de esta orden
fue entregado al almacén.

**Fecha de Inicio programada**: Es la fecha en que el MRP establece que la orden
debe ser surtida a la planta.

**Fecha de Terminación Programada**: Es la fecha en que el MRP establece que la
orden debe ser entregada al almacén.

**Fecha de Inicio Real**: Es la fecha en que la orden es liberada a la planta para ser
producida.

**Fecha de Terminación Real**: Es la fecha en que se elabora el cierre de la orden.

**Flotación Anterior** – Se utilizará posteriormente para el proceso de balanceo de la
carga de Recursos.

**Flotación Posterior** – Se utilizará posteriormente para el balanceo de la carga de
Recursos.

En el **Grupo Cantidades** se introduce la cantidad de producto a fabricar con  la Orden de Manufactura y su Unidad de Medida.

La **Cantidad del Lote** y la **Cantidad del Tamaño del lote** nos indica cuantos lotes de producción integran la OM y de que tamaño serán. Estos datos son tomados del Flujo de Trabajo de la OM. 

En el campo **Cantidad Entregada** se muestra la cantidad que ha sido entregada al almacén de producto terminado hasta el momento.

La **cantidad Rechazada**: en este campo se muestra la cantidad que no ha cubierto las  especificaciones  de  calidad  hasta  el  momento  y  que  por  lo  tanto  deberá  ser posteriormente  reprocesada  o  enviada  al  desperdicio,  en  éste  último  caso  esa cantidad se desplegará en el campo Desperdicio.

En  el  campo **Rendimiento** se  despliega  la  cantidad  de  producto  que  reúne  las especificaciones de calidad dividida entre la cantidad total de la orden a producir.

**Proyecto y Campaña** se refieren a las dimensiones estándar de Libertya.
=======
Una **Orden de Manufactura** es un documento que indica a la planta el compromiso de fabricar un producto en una cantidad establecida y en una fecha específica.

Si bien las Ordenes de anufactura sn generadas de formaq automática por el MRP, también pueden ser modificadas y/o creadas manualmente.

1. Acceder a la opción del menú **Gestión de Manufactura →  Gestión de la Producción → Orden de Manufactura**. El sistema presenta una ventana como lo muestra la Imagen 43.
2. Campos a ingresar:
	* **Compañía:** Compañía o empresa que utiliza ésta instalación. Compañía, empresa o entidad legal. No se puede compartir datos entre compañías.
	* **Organización:** Entidad organizacional dentro de la compañía. Una organización es una unidad de la compañía o entidad legal - Ej. Tiendas y departamentos.
	* **Nro. Del Documento:** Número identificador de la Orden de Manufactura. Es usualmente generado automáticamente por el sistema y determinado por el tipo del documento.
	* **Tipo Documento Destino:** Debe ser Orden de Manufactura.
	* **Activo:** El registro está activo en el sistema. Hay dos métodos para que los registros no estén disponibles en el sistema: Uno es eliminar el registro; el otro es desactivarlo. Un registro desactivado no está disponible para selección; pero está disponible para reportes.
	* **Descripción:** Descripción corta opcional del registro. Una descripción esta limitada a 255 caracteres.
	* **Artículo:** Artículo objeto de la producción asociada a esta Orden de Manufactura.
	* **Lista de Materiales:** Lista de Materiales asociada al artículo objeto de la producción asociada a esta Orden de Manufactura.
	* **Recurso:** Planta donde se realiza la producción.
	* **Flujo de Trabajo:** Flujo de trabajo o combinación de tareas, asociado al artículo objeto de la producción asociada a esta Orden de Manufactura.
	* **Almacén:** Almacén asociado al artículo objeto de la producción asociada a esta Orden de Manufactura.
	* **Prioridad:** Prioridad de un documento. La prioridad indica la importancia (alta; media; baja) de este documento.
	* **Fecha de la Orden**
	* **Fecha Prometida:** Indica la fecha en la que se espera la Orden de Manufactura este finalizada. Indica la fechaen que la orden fue prometida al cliente.
	* **Fecha de Confirmación**
	* **Fecha de la Entrega**
	* **Fecha Inicio programada:** Fecha Inicio Programada para la OM.
	* **Fecha Final Programada:** Fecha Final Programada para la OM.
	* **Fecha de Inicio:** Es la fecha cuando el primer movimiento de la orden de manufactura fue reportado, este movimiento puede ser un inventario o movimiento de labor.
	* **Fecha de Terminación:** La fecha final se usa para indicar cuando se espera que el proyecto se complete o cuando ha sido completado.
	* **Flotante Antes
	* **Flotante Despues
	* **Cantidad:** Cantidad de la Orden de Manufactura.
	* **UM:** Unidad de Medida del Producto de la Orden de Manufactura.
	* **CantidadLotes**
	* **Tamaño Cantidad Lote**
	* **Cantidad Entregada:** La Cantidad Entregada indica la cantidad de un producto que ha sido entregada.
	* **Cantidad Rechazada:** La Cantidad Rechazada indica la cantidad de un producto que ha sido rechazada.
	* **% de Rendimiento**
	* **Cantidad Desperdicio
	* **Proyecto:** Identifica un proyecto único. La ID de un proyecto es un identificador definido por el usuario para un proyecto.
	* **Estado del Documento:** El Estado del Documento indica el estado del documento en este momento. Si usted quiere cambiar el Estado del Documento; use el campo Acción del Documento.
	* **Acción en el Documento:** El estado destino del documento .
	* **Tipo de Documento:** Tipo de documento o reglas. El tipo de documento determina la secuencia del documento y las reglas de proceso.
	* **Copiar Desde**
	* **Estado Contable**
	* **Impreso**
	* **Procesado**

3. Guardar

.. figure:: _static/images/ly_om_1.png
    :alt: Orden de Manufactura
    :align: center
    :figclass: align-center

    Imagen 44: Orden de Manufactura

De forma automática, el sistema carga los datos referidos a la fórmula y flujo de trabajo definidos como se muestra en las pestañas de la ventana:

Pestaña de Fórmula

.. figure:: _static/images/ly_om_2.png
    :alt: Fórmula
    :align: center
    :figclass: align-center

    Imagen 45: Fórmula

Pestaña de Componentes de la Fórmula

.. figure:: _static/images/ly_om_3.png
    :alt: Componentes de la Fórmula
    :align: center
    :figclass: align-center

    Imagen 46: Componentes de la Fórmula

Pestaña de Flujo de Trabajo

.. figure:: _static/images/ly_om_4.png
    :alt: Flujo de Trabajo
    :align: center
    :figclass: align-center

    Imagen 47: Flujo de Trabajo

Pestaña de Actividades o Nodos del Flujo de Trabajo

.. figure:: _static/images/ly_om_5.png
    :alt: Actividades o Nodos del Flujo de Trabajo
    :align: center
    :figclass: align-center

    Imagen 48: Actividades o Nodos del Flujo de Trabajo

Pestaña de Costos asociados (se generan cuando se procesa la orden y se calculan al cerrar la orden).

.. figure:: _static/images/ly_om_6.png
    :alt: Costos
    :align: center
    :figclass: align-center

    Imagen 49: Costos
>>>>>>> fa6e9a28e75d36a2f03b7838d038b1c9c52a8176

