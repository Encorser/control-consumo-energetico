# 1.2. Requerimientos del sistema

## 1.2.1. Requerimientos funcionales

| ID | Requerimiento |
|---|---|
| RF01 | El sistema permitirá registrar manualmente recibos de CFE con fecha inicial y final del periodo facturado, consumo en kWh e importe en MXN. Antes de guardar, comprobará que los campos estén completos; que las fechas tengan formato válido y la fecha inicial no sea posterior a la final; y que consumo e importe sean valores numéricos mayores o iguales a cero. Si un dato no es válido, bloqueará el guardado e indicará qué campo debe corregirse. Si el periodo se traslapa con otro registro, mostrará una advertencia para evitar duplicidades o comparaciones ambiguas. |
| RF02 | El sistema permitirá consultar el historial y comparar el consumo y el importe de dos periodos seleccionados. Antes de comparar, verificará que ambos periodos tengan datos válidos y que sus rangos de fechas no se traslapen. Si no hay dos periodos válidos, explicará el motivo. Si las duraciones son distintas, mostrará una advertencia de que los totales corresponden a periodos de diferente duración. |
| RF03 | El sistema analizará los consumos registrados para detectar aumentos, disminuciones o igualdad entre los periodos seleccionados. Cuando detecte un aumento y los datos permitan la comparación, mostrará una recomendación general de ahorro energético mediante reglas predefinidas. No atribuirá el aumento a un aparato específico. |

## 1.2.2. Requerimientos no funcionales

| ID | Requerimiento |
|---|---|
| RNF01 | La interfaz se presentará en español, con etiquetas claras, campos identificables y mensajes de validación específicos que indiquen cómo corregir un dato. |
| RNF02 | El sistema conservará los valores capturados sin alterarlos durante las consultas. Los cálculos utilizarán únicamente datos disponibles y válidos; no inventará consumos, importes ni periodos. |

## 1.2.3. Requerimientos de datos

| ID | Requerimiento |
|---|---|
| RD01 | El sistema almacenará para cada recibo un identificador, fechas inicial y final del periodo facturado, consumo en kWh e importe en pesos mexicanos. |
| RD02 | El resultado de comparación contendrá las fechas de los dos periodos, sus duraciones en días, consumos e importes, las diferencias calculadas y, cuando aplique, una advertencia por distinta duración o traslape. La duración se muestra como contexto; no se presentará como consumo diario. |
| RD03 | Cada recomendación guardará el periodo que origina el análisis, el resultado que la activa y el mensaje mostrado al usuario. Solo se generará cuando exista una comparación válida y el consumo actual sea mayor que el anterior. |

## Criterios de aceptación para la revisión

- **CA01 — Registro válido:** las fechas son válidas, la fecha inicial no es posterior a la final, y consumo e importe son numéricos y no negativos; se permite guardar.
- **CA02 — Campos inválidos:** falta un campo, el formato de fecha no es válido, el consumo/importe no es numérico o es negativo; no se guarda y se indica la corrección.
- **CA03 — Traslape de periodos:** el rango nuevo coincide o se traslapa con un registro existente; se muestra una advertencia antes de continuar.
- **CA04 — Comparación válida:** dos periodos con rangos no traslapados se comparan y muestran sus fechas, duración, consumo e importe.
- **CA05 — Duraciones distintas:** la comparación muestra una advertencia para evitar interpretar los totales como equivalentes.
- **CA06 — Información insuficiente:** no se calcula una comparación ni se genera recomendación.
- **CA07 — Consumo mayor:** se indica el aumento y se muestra una recomendación general.
- **CA08 — Consumo igual o menor:** se informa el resultado de la comparación y no se muestra la recomendación reservada para incrementos.

> Estado: revisión del diseño aplicada el 23 de octubre de 2026. Los criterios sirven para comprobar la lógica del prototipo; no significan que exista una aplicación funcional ejecutada. La validación externa con docente o compañeros continúa pendiente.
