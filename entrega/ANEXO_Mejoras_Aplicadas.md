# Anexo de actualización: mejoras del diseño

**Proyecto:** Control de consumo energético enfocado a una casa habitación  
**Fecha:** 23 de octubre de 2026

Este anexo complementa el documento integrador y los archivos de exposición preparados previamente. Se actualiza después de una revisión interna del diseño para registrar dos mejoras incorporadas a los requisitos y al prototipo conceptual.

## Mejora 1. Validación de los recibos antes de guardar

Se definió que los campos obligatorios deben estar completos; las fechas deben ser válidas y estar en orden; consumo e importe deben ser numéricos y no negativos. Ante errores, el guardado debe bloquearse y el usuario debe recibir un mensaje que identifique qué debe corregir. También se agregó una advertencia ante intervalos duplicados o superpuestos.

## Mejora 2. Comparaciones más claras entre periodos

Se estableció que no debe generarse una conclusión si los periodos son inválidos, incompletos o se traslapan. El resultado debe mostrar las fechas y la duración de ambos periodos y advertir cuando las duraciones difieren. Los valores siguen siendo consumos totales en kWh; no se deben presentar como consumo diario.

## Evidencias vinculadas

- [Requerimientos actualizados](../docs/requerimientos.md)
- [Regla del componente inteligente](../docs/componente-inteligente.md)
- [Prototipo y maquetas de mejora](../docs/prototipo.md)
- [Maqueta de registro validado](../prototipo/mejoras/registro-validado.svg)
- [Maqueta de comparación de periodos](../prototipo/mejoras/comparacion-periodos.svg)
- [Casos de aceptación CA01–CA11](../docs/pruebas-aceptacion.md)
- [Bitácora detallada](../evidencias/mejoras-aplicadas.md)
- [Índice de evidencias E01–E10](../evidencias/README.md)

## Estado de validación

Las dos mejoras están incorporadas en la especificación y en maquetas conceptuales con criterios de aceptación definidos. No se afirma que se hayan ejecutado en una aplicación funcional ni que hayan sido aprobadas por la docente o por compañeros. La validación externa debe completarse y documentarse después de la revisión real.

Este anexo es un complemento actualizado al documento integrador y los archivos de exposición que ya se encontraban en la carpeta de entrega; no los reemplaza automáticamente.
