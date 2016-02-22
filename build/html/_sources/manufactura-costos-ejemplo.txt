************************************************
Manufactura - Ejemplo de Configuración de Costos
************************************************

**Introducción**

Se fabrica un producto **P1** cuya fórmula para una unidad de producto es la siguiente:

	* Producto **P2** - 5 unidades
	* Producto **P3** - 1 unidad
	* Producto **P4** - 5 unidades

Por otra parte el flujo de trabajo para la producción de **P1** es el siguiente:

	* Etapa 1, recurso asociado **R1**, tiempo consumido por unidad de P1 es 2 segundos.
	* Etapa 2, recurso asociado **R2**, tiempo consumido por unidad de P1 es 6 segundos.

Para poder sacar el costo de una Orden de Manufactura de **P1**, necesitamos previamente, configurar los elementos de costos de los componentes de la fórmula de **P1**, y de los recursos del flujo de trabajo de **P1**.

**Pasos a Paso**

1. Configurar los **Tipo de Coste** a ser utilizados.

2. Configurar los **Elemento de Coste** a ser utilizados.

3. Configurar para cada **Artículo** de la fórmula (P2, P3 y P4) un registro de Coste de Artículo, definiendo la asociación entre:
	* Esquema Contable.
	* Almacén.
	* Tipo de Coste.
	* Elemento de Coste.

4. Configurar para cada **Recurso** (representado por una Artículo) del flujo de trabajo (R1 y R2) un registro de Coste de Artículo, definiendo la asociación entre:
	* Esquema Contable.
	* Almacén.
	* Tipo de Coste.
	* Elemento de Coste.

5. Configurar en la pestaña de **Contabilidad**, de la ventana **Subfamilia** del Artículo (lo mismo vale para los Recursos), el **Tipo de Coste** que va a tomar el sistema para el cálculo, que debe coincidir con el configurado en Coste de Artículo. para cada producto de la fórmula (P2, P3 y P4). Esto permite que cada Subfamilia, pueda tomar un método de costeo diferente. En caso de querer un único método de costeo, hacer esta configuración a nivel de **Esquema Contable**. Este último tipo de configuración, se usaría por ejemplo en caso de usar como método de costeo único **Costo Estándar**.

6. Cuando de procesa una orden (proceso Imprimir y Liberar Orden), se crean los registros de costos en función de lo configurado en los pasos 3 y 4.

7. Agregar los costos manuales vinculados a la Orden de Manufactura (principalmente **Costos Indirectos**).

8. Ejecutar el proceso de **Cerrar la Orden de Manufactura**, esto entre otras cosas procesa el cálculo de costos directos asociados a la Orden de Manufactura.





