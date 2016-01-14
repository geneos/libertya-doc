*****************************************************
Manufactura - Checklist para correr el proceso de MRP
*****************************************************

Consideraciones Generales
-------------------------

    * Tanto el producto padre, como todos los componentes del mismo, tienen que tener Datos de Planificación de producto.
    * Al menos tenemos que tener un recurso de tipo Planta.
    * Establecer el horizonte de la planta en un valor > 0, tener en cuenta que esto valida las posibles demandas futuras, o sea si tengo una demanda más allá del horizonte no van a ser explotadas.
    * Tener un pronóstico / demanda para el período actual
    * Correr el proceso Verificar Lista de Materiales para cada familia

Si el componente es comprado
----------------------------

    * En la ventana **Artículo**, pestaña **Artículo**, desmarcar el casilla de verificación **Es Manufacturado** y marcar el check **Comprado**.
    * En la ventana **Artículo**, pestaña **Compras**, cargar un registro con un proveedor asociado por defecto.
    * En la ventana **Datos de Planificación del Producto**, pestaña **Datos de Planificación**, cargar datos que correspondan:
        * Recurso (la Planta donde se va a producir).
        * Almacén.
        * Política de Ordenamiento.
        * Tiempos (no es mandatorio, dependen de cada producto y de la Política de Ordenamiento).
        * Cantidades (no es mandatorio, dependen de cada producto y de la Política de Ordenamiento).
        * Marcar el check Crear Plan.


Si el componente es fabricado
-----------------------------

    * En la ventana **Artículo**, pestaña **Artículo**, marcar el casilla de verificación **Es Manufacturado** y desmarcar el casilla de verificación **Comprado**..
    * En la ventana **Datos de Planificación del Producto**, pestaña **Datos de Planificación**, cargar datos que correspondan:
        * Recurso (la Planta donde se va a producir).
        * Almacén.
        * Lista de Materiales.
        * Flujo de Trabajo
        * Política de Ordenamiento.
        * Tiempos (no es mandatorio, dependen de cada producto y de la Política de Ordenamiento).
        * Cantidades (no es mandatorio, dependen de cada producto y de la Política de Ordenamiento).
        * Marcar el casilla de verificación Crear Plan.
