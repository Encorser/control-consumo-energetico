# 3. Componente inteligente

El sistema contará con una función de análisis que permitirá comparar el consumo eléctrico registrado en los recibos de CFE e identificar incrementos entre periodos de facturación. A partir de esta comparación, se generarán recomendaciones generales de ahorro energético mediante reglas predefinidas, sin necesidad de implementar un modelo avanzado de inteligencia artificial.

## 3.1. ¿Qué problema resuelve?
La función busca facilitar la identificación de aumentos en el consumo eléctrico de una casa habitación. Al registrar los recibos manualmente, el usuario podrá consultar las variaciones del consumo y recibir una recomendación cuando se detecte un incremento respecto al periodo anterior.

## 3.2. ¿Qué datos utiliza?
- Consumo eléctrico de cada periodo, expresado en kilowatt-hora (kWh).
- Fechas de inicio y fin del periodo facturado.
- Importe del recibo en pesos mexicanos.
- Consumo registrado en el periodo anterior, cuando exista.

## 3.3. ¿Qué procesamiento realiza?
El sistema identificará los periodos de facturación registrados y comparará el consumo eléctrico en kWh del periodo seleccionado con el del periodo anterior. Calculará la diferencia entre ambos consumos para determinar si la cantidad de energía registrada aumentó, disminuyó o permaneció igual.

Cuando el consumo del periodo actual sea superior al del periodo anterior, el sistema mostrará una recomendación general de ahorro energético. Esta decisión se realizará mediante una regla predefinida, sin necesidad de implementar inteligencia artificial avanzada.

Si no existe un registro anterior suficiente para efectuar la comparación, el sistema informará al usuario que todavía no es posible determinar la variación del consumo.

## 3.4. ¿Qué resultado genera?
El sistema mostrará el resultado de la comparación entre los periodos registrados, indicando si el consumo aumentó, disminuyó o permaneció igual. También podrá presentar la diferencia de consumo en kWh y la variación del importe facturado cuando existan datos suficientes.

Cuando detecte un incremento en el consumo eléctrico, mostrará una recomendación general para fomentar el ahorro de energía en la vivienda. Las recomendaciones serán orientativas y no identificarán aparatos específicos responsables del incremento.

## Regla acordada
Si el consumo actual en kWh es mayor que el consumo del periodo anterior, el sistema genera una recomendación. Si no existe un periodo anterior suficiente, no realiza comparación y comunica esa situación.

> Nota: cuando los periodos facturados tienen distinta duración, el resultado refleja el consumo total registrado en cada periodo y no necesariamente el consumo diario.
