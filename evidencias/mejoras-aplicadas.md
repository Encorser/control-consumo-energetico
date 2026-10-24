# Bitácora de mejoras aplicadas

**Proyecto:** Control de consumo energético enfocado a una casa habitación  
**Fecha de revisión interna:** 23 de octubre de 2026  
**Tipo de cambio:** precisión de requisitos y prototipo conceptual.

## Contexto

Una revisión interna de los requisitos y de la lógica descrita identificó dos áreas que convenía precisar para hacer el diseño más verificable. Se aplicaron los cambios a la documentación y se añadieron dos maquetas SVG complementarias. Esta revisión no debe confundirse con retroalimentación del docente o de compañeros: esa validación externa sigue pendiente.

## M01. Validar los datos antes de guardar un recibo

**Problema detectado en la especificación anterior:** se mencionaba validación general, pero no se definían las condiciones para fechas invertidas, datos no numéricos o importes/consumos negativos.

**Cambio aplicado:** RF01 y RNF01 ahora especifican campos obligatorios, fechas válidas, fecha inicial no posterior a la final, consumo e importe numéricos y no negativos, bloqueo del guardado ante errores y mensajes asociados al campo que debe corregirse. También se añadió una advertencia ante periodos que coincidan o se traslapen con otro registro.

**Motivo:** convertir un requisito general en una condición verificable y reducir capturas inválidas o confusas.

**Artefactos actualizados:**
- [Requerimientos](../docs/requerimientos.md)
- [Maqueta de registro validado](../prototipo/mejoras/registro-validado.svg)
- [Casos de aceptación CA01–CA06](../docs/pruebas-aceptacion.md)

## M02. Precisar las condiciones de comparación

**Problema detectado en la especificación anterior:** no se explicaba qué hacer con rangos superpuestos ni cómo comunicar las diferencias de duración entre periodos facturados.

**Cambio aplicado:** RF02, RD02 y la regla de análisis ahora requieren periodos válidos y sin traslape, muestran las fechas y duración de cada periodo, y advierten cuando las duraciones difieren. Se conservan los consumos totales en kWh y no se les denomina consumo diario.

**Motivo:** evitar conclusiones basadas en periodos superpuestos o interpretar como equivalentes totales de diferente duración.

**Artefactos actualizados:**
- [Requerimientos](../docs/requerimientos.md)
- [Componente inteligente](../docs/componente-inteligente.md)
- [Maqueta de comparación](../prototipo/mejoras/comparacion-periodos.svg)
- [Casos de aceptación CA07–CA11](../docs/pruebas-aceptacion.md)

## Estado y límites

| Elemento | Estado actual |
|---|---|
| Requisitos actualizados | Aplicado en documentación |
| Regla de comparación detallada | Aplicado en documentación |
| Dos maquetas de interfaz | Creadas como artefactos SVG complementarios |
| Casos de aceptación | Definidos; ejecución pendiente |
| Pruebas en aplicación funcional | No realizadas; no hay sistema funcional en alcance |
| Retroalimentación de docente o compañeros | Pendiente de obtener y registrar |
| Confirmación externa de las mejoras | Pendiente |

Los cambios son mejoras reales de especificación y diseño. No se afirma que el software se haya implementado ni que las mejoras hayan sido aprobadas por terceros. La revisión externa puede confirmar, corregir o generar cambios adicionales.
