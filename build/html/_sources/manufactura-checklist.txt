*****************************************************
Manufactura - Checklist para correr el proceso de MRP
*****************************************************

* Tanto el producto padre, como todos los componentes del mismo, tienen que tener Datos de Planificación de producto.

----------------------------

Si el componente es comprado:
#############################
* Desmarcar el check Es Manufacturado en artículo
* Marcar Comprado en artículo
* Debe tener proveedor asociado y código de producto del prov.
* Cargar datos de planificación:
    * Recurso (planta)
    * Almacén
    * Tiempos (no es mandatorio)
    * Marcar el check Crear plan


Si el componente es fabricado:
##############################
* Desmarcar el check Comprado en el artículo
* Marcar el check Es Manufacturado en artículo
* Cargar datos de planificación:
    * Lista de Materiales
    * Flujo
    * Recurso (planta)
    * Almacén
    * Tiempos (no es mandatorio)
    * Marcar el check **Crear plan**

-----------------------------------

* Al menos tenemos que tener un recurso de tipo Planta
* Establecer el horizonte de la planta en un valor > 0, tener en cuenta que esto valida las posibles demandas futuras, o sea si tengo una demanda más allá del horizonte no van a ser explotadas.
* Tener un pronóstico / demanda para el período actual
* Correr el proceso Verificar Lista de Materiales para cada familia