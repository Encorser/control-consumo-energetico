# 10. Validación del proyecto

**Proyecto:** Control de consumo energético enfocado a una casa habitación  
**Estado:** dos mejoras incorporadas a la documentación y al prototipo conceptual; validación externa pendiente  
**Tipo de revisión realizada:** revisión interna del diseño y definición de criterios de aceptación. No equivale a aprobación de la docente ni a ejecución de pruebas de una aplicación funcional.

## 10.1. Objetivo

Revisar que el problema, los requerimientos, el flujo del prototipo y la regla de análisis sean claros y coherentes. La revisión interna se utilizó para concretar dos áreas de mejora; aún se requiere la revisión con docente o compañeros para obtener retroalimentación externa.

## 10.2. Estado previo y actual

Las listas individuales preparadas para los tres requerimientos funcionales (RF01–RF03), dos no funcionales (RNF01–RNF02) y tres de datos (RD01–RD03) continúan siendo preliminares. Se actualizaron la especificación de requerimientos, la lógica del componente inteligente y el diseño conceptual de pantallas para aclarar las validaciones y los casos límite.

Las mejoras se documentan como cambios realmente incorporados en los artefactos de diseño. No se presentarán como comentarios recibidos de terceros ni como pruebas de software ejecutadas.

## 10.3. Mejoras aplicadas

| ID | Área de mejora identificada en la revisión interna | Cambio incorporado | Motivo | Evidencia |
|---|---|---|---|---|
| M01 | Los criterios de captura eran generales y podían dejar dudas sobre valores y fechas inválidos. | RF01 y RNF01 especifican campos obligatorios, validación de fechas, consumo e importe numéricos no negativos, mensajes por campo y bloqueo del guardado ante errores. Se añadió advertencia de traslape de periodos. | Reducir errores de captura y hacer el requisito verificable. | [Requerimientos](requerimientos.md), [maqueta de registro](../prototipo/mejoras/registro-validado.svg), [pruebas de aceptación](pruebas-aceptacion.md). |
| M02 | La regla de comparación no definía con suficiente precisión los periodos superpuestos ni la diferencia de duración. | RF02 y la regla de análisis impiden concluir con periodos traslapados, requieren datos válidos, muestran la duración de cada periodo y advierten si es distinta. Se mantienen los totales en kWh sin llamarlos consumo diario. | Evitar comparaciones ambiguas o interpretaciones incorrectas de periodos de diferente duración. | [Componente inteligente](componente-inteligente.md), [maqueta de comparación](../prototipo/mejoras/comparacion-periodos.svg), [pruebas de aceptación](pruebas-aceptacion.md). |

## 10.4. Aspectos todavía pendientes de validación externa

| Aspecto | Evidencia que debe obtenerse | Estado |
|---|---|---|
| Comprensión del problema y usuario | Comentarios reales de docente o compañeros | Pendiente |
| Comprensión y viabilidad de requerimientos | Revisión de RF01–RF03, RNF01–RNF02 y RD01–RD03 | Pendiente |
| Correspondencia de prototipo y lógica | Revisión de las cuatro pantallas base y las maquetas complementarias | Pendiente |
| Adecuación de las dos mejoras | Confirmación o corrección a partir de comentarios reales | Pendiente |
| Exposición individual | Presentación, justificación de decisiones y respuestas a preguntas | Pendiente de realizar |

## 10.5. Procedimiento para completar la validación

1. Presentar el problema, requerimientos, cuatro pantallas y dos maquetas complementarias al grupo y/o docente.
2. Registrar quién revisó el proyecto, la fecha y las observaciones textuales o resumidas fielmente.
3. Preguntar si las validaciones de captura son suficientes y si las reglas para periodos superpuestos o de distinta duración son comprensibles.
4. Ajustar los artefactos si la retroalimentación señala cambios adicionales.
5. Actualizar esta sección y adjuntar la evidencia permitida por la actividad.

## 10.6. Registro de retroalimentación externa

| Fecha | Persona o grupo revisor | Observación recibida | Cambio derivado | Evidencia |
|---|---|---|---|---|
| Pendiente | Pendiente | No se ha recibido/registrado todavía | Pendiente de confirmar | Pendiente |

## 10.7. Alcance de las pruebas de aceptación

Los escenarios de [pruebas de aceptación](pruebas-aceptacion.md) describen entradas y resultados esperados para comprobar la lógica. Al tratarse de un prototipo conceptual, no se afirma que un sistema de software ejecutable haya superado pruebas. La validación externa sigue pendiente.
