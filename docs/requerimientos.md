# 1.2. Requerimientos del sistema

## 1.2.1. Requerimientos funcionales

| ID | Requerimiento |
|---|---|
| RF01 | El sistema permitirá registrar manualmente los recibos de CFE, incluyendo las fechas del periodo facturado, el consumo eléctrico en kWh y el importe en pesos mexicanos. Validará que los campos obligatorios estén completos antes de guardar la información. |
| RF02 | El sistema permitirá consultar el historial de recibos registrados y comparar el consumo eléctrico y los importes entre diferentes periodos de facturación. Cuando no existan registros suficientes, informará al usuario que no es posible realizar la comparación. |
| RF03 | El sistema analizará los consumos registrados para detectar incrementos o disminuciones entre periodos consecutivos. Cuando detecte un incremento, mostrará una recomendación general de ahorro energético basada en reglas predefinidas. |

## 1.2.2. Requerimientos no funcionales

| ID | Requerimiento |
|---|---|
| RNF01 | El sistema deberá presentar su interfaz en español, con etiquetas claras, campos identificables y mensajes comprensibles para facilitar su uso por una persona sin conocimientos técnicos especializados. |
| RNF02 | El sistema deberá conservar los valores registrados de consumo e importe sin alterarlos durante las consultas y comparaciones. Los resultados deberán calcularse utilizando los datos disponibles, sin generar valores de consumo inexistentes. |

## 1.2.3. Requerimientos de datos

| ID | Requerimiento |
|---|---|
| RD01 | El sistema deberá almacenar los datos de los recibos de CFE, incluyendo un identificador, las fechas del periodo facturado, el consumo en kWh y el importe en pesos mexicanos. |
| RD02 | El sistema deberá disponer de los resultados de los análisis realizados, incluyendo los periodos comparados, los consumos registrados, las diferencias detectadas y la variación de los importes cuando existan datos suficientes. |
| RD03 | El sistema deberá registrar las recomendaciones generadas, incluyendo el resultado del análisis que las origina, el mensaje presentado al usuario y el periodo al que corresponden. |

> Estado: propuesta de requerimientos acordada en la conversación; pendiente de validación final.
