# 4. Prototipo

**Estado del diseño:** realizado. El archivo PowerPoint de cuatro pantallas está incorporado al repositorio en la carpeta `prototipo/` y se revisó su contenido para confirmar que corresponde a las pantallas descritas a continuación.

**Archivo del prototipo:** [`(Presentacion) prototipo_control_consumo_energetico.pptx`](../prototipo/%28Presentacion%29%20prototipo_control_consumo_energetico.pptx).

El prototipo tiene finalidad demostrativa y no necesita conectarse con una base de datos real ni con CFE.

## Pantalla 1. Panel principal
**Objetivo:** presentar un resumen del consumo eléctrico registrado y facilitar el acceso a las funciones del sistema.

**Elementos:** nombre del sistema, consumo e importe del último periodo, variación respecto al periodo anterior cuando exista información y accesos para registrar, consultar historial y revisar el análisis.

**Interacción:** al seleccionar una opción, el usuario accede a la pantalla correspondiente.

## Pantalla 2. Registro de recibo de CFE
**Objetivo:** permitir la captura manual de un recibo.

**Elementos:** fecha de inicio y fin del periodo facturado, consumo en kWh, importe en pesos y botones para guardar o cancelar.

**Interacción:** el usuario introduce los datos y guarda. El sistema verifica que los campos obligatorios estén completos y sean válidos; de lo contrario, muestra un mensaje de corrección.

## Pantalla 3. Historial y comparación
**Objetivo:** facilitar la consulta de recibos y la comparación entre periodos.

**Elementos:** tabla con periodo, consumo en kWh e importe; selección de periodos y área de resultados con diferencias.

**Interacción:** el usuario selecciona los periodos y el sistema muestra las diferencias calculadas. Si no existen registros suficientes, informa que no es posible comparar.

## Pantalla 4. Análisis y recomendaciones
**Objetivo:** presentar los resultados del componente inteligente.

**Elementos:** consumo actual y anterior, diferencia en kWh, estado de la variación, variación del importe cuando sea posible y recomendación general cuando el consumo aumente.

**Interacción:** si el consumo actual es superior al anterior, aparece una recomendación. Si no hay un periodo previo, el sistema informa que no puede comparar.

## Datos demostrativos
Las cifras del prototipo son hipotéticas. Se muestran solo para ilustrar las pantallas y deben etiquetarse como ejemplos, no como datos reales de CFE.

## Evidencias pendientes
- Guardar una captura de la carpeta `prototipo/` en GitHub donde se vea el archivo PPTX.
- Guardar una captura de vista general de las cuatro pantallas, por ejemplo, el panel de miniaturas de PowerPoint.
