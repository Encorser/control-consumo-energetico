# 3. Componente inteligente

El sistema cuenta, a nivel de diseño, con una función de análisis basada en reglas predefinidas. Compara los consumos registrados en recibos de CFE y ayuda a identificar aumentos, disminuciones o igualdad entre periodos. No es un modelo avanzado de inteligencia artificial y no atribuye cambios a aparatos específicos.

## 3.1. ¿Qué problema resuelve?

Facilita que el usuario detecte variaciones entre registros de consumo doméstico. Cuando una comparación válida demuestra un aumento, el sistema presenta una recomendación general de ahorro.

## 3.2. Datos de entrada

- Consumo de los periodos seleccionados, expresado en kWh.
- Fechas inicial y final de cada periodo.
- Importe de cada recibo en MXN.
- Duración de cada periodo, calculada a partir de sus fechas.
- Confirmación de que los periodos son válidos y no se traslapan.

## 3.3. Regla de procesamiento revisada

1. Verificar que existan dos registros completos y con valores numéricos válidos.
2. Confirmar que las fechas estén en orden y que los rangos comparados no se traslapen.
3. Calcular la duración de cada periodo y mostrar las fechas completas.
4. Comparar los consumos totales en kWh y los importes registrados.
5. Si las duraciones son distintas, mostrar una advertencia visible: **“Los periodos tienen distinta duración; compara los consumos totales con cautela.”** No convertir ni etiquetar esos totales como consumos diarios.
6. Clasificar el resultado como aumento, disminución o sin cambio.
7. Generar una recomendación general únicamente cuando el consumo del periodo actual sea mayor y la comparación sea válida.
8. Si faltan datos o los periodos se traslapan, no presentar una conclusión; explicar qué debe revisarse.

## 3.4. Resultados esperados

El resultado muestra las fechas de ambos periodos, duración en días, consumo total, importe y diferencias. Cuando aplique, incorpora una advertencia por diferente duración. Si el consumo aumenta, aparece una recomendación general, por ejemplo revisar hábitos de uso de iluminación y desconectar equipos que no se estén utilizando. La recomendación es orientativa y no afirma cuál aparato causó el aumento.

## 3.5. Ejemplos para comprobar la regla

| Caso | Entrada | Resultado esperado |
|---|---|---|
| Hay un periodo anterior y los rangos no se traslapan | Periodo actual 420 kWh; anterior 386 kWh | Diferencia de +34 kWh y recomendación general. |
| El consumo actual es menor | Actual 360 kWh; anterior 386 kWh | Se informa disminución; no se activa la recomendación por aumento. |
| Ambos consumos son iguales | Actual 386 kWh; anterior 386 kWh | Se informa que no hubo cambio. |
| Los periodos tienen distinta duración | Actual 60 días; anterior 59 días | Se muestran ambas duraciones y una advertencia sobre la comparación de totales. |
| No hay dos registros válidos o las fechas se traslapan | Un periodo o rangos superpuestos | No se emite conclusión; se informa qué dato corregir o qué periodo elegir. |

> Estos ejemplos son datos hipotéticos para revisar el diseño, no recibos reales ni resultados de ejecución de software. La regla fue precisada en la revisión interna del diseño; la revisión real con docente o compañeros permanece pendiente.
