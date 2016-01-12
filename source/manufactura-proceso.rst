Ejecución del MRP
=================

El MRP es un proceso que combina las Listas de Materiales, datos de existencia, órdenes abiertas de compra y manufactura y el Plan Maestro de Producción  para calcular el requerimiento de los materiales. Genera órdenes planeadas para balancear la demanda de productos con  su  abastecimiento  y  emite  recomendaciones  para  recibir  el  material  en cantidades  y  fechas  para  cubrir  los  requerimientos  del  PMP  de  la  manera  más eficiente. El proceso MRP debe completarse siguiendo los paso detallados a continuación:

**Paso 1: Niveles inferiores**
Este proceso identifica el nivel más bajo de un producto dentro de cualquier estructura. Se utiliza para el cálculo del requerimiento neto de un producto una vez que se han calculado todos  los  requerimientos  brutos  del  producto  hasta  la  estructura  que  utiliza  el producto en el nivel más bajo.

**Paso 2: Crear Registros MRP** 
Antes de comenzar con el proceso se deben proveer los parámetros 

**AVISOS**
Cuando el proceso finaliza se visualiza una ventana con posibles errores.

**Paso 3: Calcular Plan de Materiales**
Cumplidos los pasos anteriores, podemos calcular el plan de materiales. En el cálculo de plan de materiales, se utilizan los datos provistos por el PMP, es decir los datos maestros que relacionan las Listas de Materiales, los recursos de manufactura y los flujos de trabajo y distribución. Durante este proceso se establece si las existencias y las requisiciones existentes satisfacen las necesidades para la producción.

Cuando este proceso finaliza, se muestran las Órdenes de Manufactura, las Requisiones y los Avisos que fueron generados. 

**Revisar y confirmar la producción**
=====================================
 
Luego de la ejecución y especialmente, si se obtuvieron Avisos, se deben verificar los resultados mediante las siguientes opciones:

**Consulta del MRP**

Al realizar una Consulta de MRP, se pueden verificar las cantidades comprometidas tanto por pronóstico como por Orden de Manufactura para un producto determinado. Ir a Gestión de Manufactura, MRP, Consulta de MRP. En esta ventana se puede indicar el producto para obtener un listado de toda la demanda del producto, ya sea generadas tanto por órdenes de venta, como por pronósticos.

**Avisos del MRP**
Contiene un grupo de mensajes generados por el proceso MRP. Indica al usuario que acciones son necesarias para poder alcanzar el Planeamiento de Producción correctamente.


+------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|   MRP-001  | Cantidad Inicial menor que cero. Es negativa.                                                                                                                                                                                                                                   |
+------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|   MRP-020  | Un pedido de aprovisionamiento debería ser creado para satisfacer un balance negativo proyectado. Este mensaje sólo es generado si "Crea Plan" es NO o si aparece un nuevo requerimiento de última hora.                                                                        |
+------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|   MRP-030  | Indica que un pedido de aprovisionamiento va ser procesado antes de ser necesitado y debería de ser retrasado, o bien reprogramado a un estado anterior.                                                                                                                        |
+------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|   MRP-040  | Indica que un pedido de aprovisionamiento programado será entregado con mucha posterioridad a ser necesario y que debería de ser reprogramado a una fecha anterior o reprocesador a un estado posterior.                                                                        |
+------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|   MRP-050  | Indica que un pedido de aprovisionamiento ya no es necesario y debería de ser borrado.                                                                                                                                                                                          |
+------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|   MRP-060  | Indica que un pedido programado debería de ser lanzado.                                                                                                                                                                                                                         |
+------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|   MRP-070  | Lanzar pedido retrasado. Indica que un pedido de aprovisionamiento no fue lanzado cuando debía, y debe de ser lanzado o aprovisionado ahora, o la demanda reprogramada para una fecha posterior.                                                                                |
+------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|   MRP-080  | Cantidad por debajo del minimo. Indica que un pedido de aprovisionamiento fue creado por una cantidad inferior a la cantidad mínima prevista en la planificación de stock del producto.                                                                                         |
+------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|   MRP-090  | Cantidad por encima del máximo. Indica que un pedido de aprovisionamiento fue creado por una cantidad mayor que la cantidad máxima prevista en la planificación de stock del producto.                                                                                          |
+------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|   MRP-100  | Indica que hay un requerimiento de material no satisfecho dentro de la planificación de stock para este producto. Debería ser programado manualmente o expedir pedidos de aprovisionamiento para cumplir con la demanda o posponer los requerimientos que crearon dicha demanda.|
+------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|   MRP-110  | No existe almacén de demanda. En la planificación del producto no figura la demanda.                                                                                                                                                                                            |
+------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|   MRP-120  | No existe almacén de suministros. En la planificación del producto no figura los suministros.                                                                                                                                                                                   |
+------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
