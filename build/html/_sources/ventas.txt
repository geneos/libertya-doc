*****************
Módulo de Ventas
*****************

**Datos previos necesarios**


1. Clientes
2. Artículos
3. Lista de Precios de Compras
4. Medios de Cobro
5. Configuración de TPV
6. Centros de Costos


TPV
---

La terminal de Punto de Venta (TPV) permite el ingreso rápido de las facturas de clientes.

.. figure:: _static/images/ly_tpv_19.png
    :alt: TPV
    :align: center
    :figclass: align-center

    Imagen 19: TPV – Ingreso de Ítem

Acceder con el perfil "Ventas" a la opción del menú, menú TPV →  TPV, el sistema presenta una ventana como lo muestra la Imagen 19.

Las referencias para el ingreso de la información de la compra son las siguientes:

1. Es el área de selección de los productos y cantidades (la tecla Enter sirve para fijar el producto y la cantidad ingresando la línea al pedido).
2. Es el área de ingreso del viaje, origen, destino (se mantienen los datos entre diferentes facturas, compartiendo los datos anteriormente registrados, para agilizar la carga de todas las facturas de un viaje) y valor declarado.
3. Es el área donde va quedando el detalle de las líneas de facturas, tiene una columna editable para ingresar la información de remitente asociada a cada línea.
4. Es el área de funciones:

 1. F6: para acceder a cambiar información de cantidades y precios de los productos.
 2. F8: para cambiar a la pantalla de selección de Cliente y Medio de Pago. También puede usarse el botón Cobrar.

La segunda parte de la transacción de ventas consiste en seleccionar el cliente y la forma de cobro.

1. Con el botón Cobrar o con F8 accedemos al siguiente paso de la factura que es la selección del Cliente y la Forma de Pago, el sistema presenta una ventana como lo muestra la Imagen 20.

.. figure:: _static/images/ly_tpv_20.png
    :alt: TPV
    :align: center
    :figclass: align-center

    Imagen 20: TPV – Ingreso de datos de Cobro

Las referencias para el ingreso de la información del cliente y la forma de pago son las siguientes:

 1. Es el área de selección del cliente. Se ingresa la información en el campo o se accede a la ventana de búsqueda.
 2. Es el área de ingreso de la forma de cobro, en este caso siempre va a ser Crédito.
 3. Acceso al botón para confirmar la operación (botón Cobrar o F12).

Una vez confirmado el sistema emite el comprobante correspondiente.


Cobranzas
---------
Permite registrar el cobro a un cliente.

1. Acceder con el perfil "**Administración**" a la opción del menú, menú Pagos →  Orden de Pago, el sistema presenta una ventana como lo muestra la Imagen 21.
2. **Cabecera** → Campos a ingresar:
    - Entidad Comercial
    - Tipo de documento (determina el Nro. Documento)
    - Fecha del Recibo
3. **Selección de Cobro** → Campos a ingresar: 
    - Seleccionar si es Cobro Normal o Cobro Adelantado (sin asignación de facturas)
    - Seleccionar Punto de Venta.
    - Seleccionar si se muestran todos los documentos o los vencidos a una fecha.	
    - Indicar si se cobra todo lo pendiente o indicar en la columna a pagar el monto de la las facturas seleccionadas para pagar.
    - Con el botón Siguiente o F8 se avanza a la siguiente sección.
4. **Forma de Cobro** (Imagen 22) → Campos a ingresar:
    - Moneda
    - Tipo de Cobro/Pago
    - Datos correspondientes al tipo de cobro.
    - Guardar Cambios o F9

    Repetir los últimos dos pasos en casos de cobrar con diferentes medios de cobro.
    Una vez que el Saldo sea 0 completa con el botón **Emitir Recibo** o F8

.. figure:: _static/images/ly_ventas21.png
    :alt: Cobranzas – Ingreso de comprobantes a cobrar
    :align: center
    :figclass: align-center

    Imagen 21: Cobranzas – Ingreso de comprobantes a cobrar

.. figure:: _static/images/ly_ventas22.png
    :alt: Cobranzas – Ingreso de medios de cobro
    :align: center
    :figclass: align-center

    Imagen 22: Cobranzas – Ingreso de medios de cobro


Informes
--------

**Cuenta Corriente**

Permite ver la información consolidada, de la cuenta corriente de un Cliente.

1. Acceder con el perfil "Administración" a la opción del menú, menú Informes de Cobros y Pagos →  Informe de Cuenta Corriente, el sistema presenta una ventana como lo muestra la Imagen 23.
2. Parámetros del informe (Imagen 23) → Campos a ingresar:
    - Entidad Comercial
    - Organización (por defecto lo que viene)
    - Rango de Fechas
    - Tipo de Documentos
    - Tipo de Reporte (Cliente / Proveedor)
3. Emitir informe (Imagen 24) con el botón verde.
    
.. figure:: _static/images/ly_informe_23.png
    :alt: TPV
    :align: center
    :figclass: align-center

    Imagen 23: Informe de Cta. Cte. - Parámetros

.. figure:: _static/images/ly_informe_24.png
    :alt: TPV
    :align: center
    :figclass: align-center

    Imagen 24: Informe de Cta. Cte. - Resultados


    