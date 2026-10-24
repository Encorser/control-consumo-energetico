# Casos de aceptación del diseño

**Proyecto:** Control de consumo energético en una casa habitación  
**Fecha de elaboración:** 23 de octubre de 2026  
**Estado:** casos de prueba especificados para el prototipo conceptual; no son evidencia de ejecución de una aplicación funcional.

Estos casos concretan dos mejoras de diseño: validación de entrada en el registro de recibos y comparación segura entre periodos. Deben comprobarse cuando se pruebe o implemente el sistema.

## M01. Validación del registro

| ID | Condición o entrada | Resultado esperado | Estado |
|---|---|---|---|
| CA01 | Campos completos; fechas válidas y en orden; consumo 420 kWh e importe 1050 MXN | El formulario permite guardar el recibo. | Criterio definido; ejecución pendiente |
| CA02 | Falta consumo o importe | No guarda y señala el campo obligatorio. | Criterio definido; ejecución pendiente |
| CA03 | Texto no numérico en consumo o importe | No guarda y explica el formato esperado. | Criterio definido; ejecución pendiente |
| CA04 | Consumo o importe negativo | No guarda e indica que el valor no puede ser negativo. | Criterio definido; ejecución pendiente |
| CA05 | Fecha inicial posterior a la final | No guarda y muestra el mensaje de orden de fechas. | Criterio definido; ejecución pendiente |
| CA06 | El intervalo coincide o se traslapa con otro recibo | Muestra una advertencia antes de permitir continuar. | Criterio definido; ejecución pendiente |

## M02. Comparación de periodos

| ID | Condición o entrada | Resultado esperado | Estado |
|---|---|---|---|
| CA07 | Dos periodos válidos y no traslapados: actual 420 kWh, anterior 386 kWh | Muestra la diferencia de +34 kWh y una recomendación general por aumento. | Criterio definido; ejecución pendiente |
| CA08 | Actual 360 kWh, anterior 386 kWh | Muestra disminución de 26 kWh; no activa la recomendación por aumento. | Criterio definido; ejecución pendiente |
| CA09 | Actual y anterior con 386 kWh | Indica que no hubo cambio; no activa la recomendación por aumento. | Criterio definido; ejecución pendiente |
| CA10 | Los periodos se traslapan o falta uno de los registros | No genera una conclusión y explica que debe corregirse la selección o capturarse el registro faltante. | Criterio definido; ejecución pendiente |
| CA11 | Los periodos tienen diferente duración | Muestra la duración de ambos y advierte que los consumos totales deben compararse con cautela. No los presenta como consumo diario. | Criterio definido; ejecución pendiente |

## Criterio de cierre

Para marcar un caso como aprobado, se deberá ejecutar contra la aplicación o prototipo interactivo disponible y registrar resultado, fecha y evidencia. Hasta entonces, la tabla documenta resultados esperados, no pruebas superadas.
