*********************
Módulo de Manufactura
*********************

El módulo de Manufactura se basa en MRP (Material Resource Plannig).

El MRP, consiste esencialmente, en un cálculo de necesidades netas de los artículos
(productos terminados, productos intermedios, materias primas) introduciendo un factor nuevo, no considerado en los métodos tradicionales de gestión de stocks, que es el plazo de fabricación o plazo de entrega en la compra de cada uno de los artículos, lo que en definitiva conduce a modular a lo largo del tiempo las necesidades, ya que indica la oportunidad de fabricar (o aprovisionar) los componentes, con la  debida planificación respecto a su utilización en la fase siguiente de fabricación.

**Datos utilizados por el MRP**

Fuentes principales

1. Plan Maestro detallado de Producción, que nos dice que productos finales hay que fabricar y en que plazos de entrega.
2. Lista de Materiales, indica de que partes o componentes se forma cada unidad de los productos intermedios y terminados, permitiendo calcular las cantidades de cada componente necesarias para fabricarlos.
3. Estado del Stock, permite conocer las cantidades disponibles de cada artículo y por diferencia, las cantidades que deben comprarse.

Fuentes complementarias

1. Órdenes de Producción en curso, deben considerarse como futuras disponibilidades de producto, siempre y cuando las fechas de finalización de las órdenes coincidan con los plazos en los que se requieren los productos.
2. Órdenes de Compra en curso, deben considerarse como futuras disponibilidades de producto, siempre y cuando las fechas de entrega de las órdenes coincidan con los plazos en los que se requieren los productos.

**Síntesis del Proceso MRP**

.. image:: _static/images/ly_mrp.png
    :alt: Síntesis MRP

*Imagen N*


Contenidos:

.. toctree::
   :maxdepth: 2

   manufactura-flujos
   manufactura-bom
   manufactura-plan
   manufactura-pronostico
   manufactura-proceso
   manufactura-om
   manufactura-operaciones
   manufactura-informes

