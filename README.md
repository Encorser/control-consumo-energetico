# Control de consumo energético en una casa habitación

Proyecto académico de la materia **Gestión de Proyectos de Software**.

## Descripción
Sistema propuesto para una vivienda familiar hipotética ubicada en Tuzamapan, Xalapa, Veracruz, México. El usuario registrará manualmente recibos de la Comisión Federal de Electricidad (CFE), incluyendo el periodo facturado, consumo en kWh e importe en MXN.

## Funcionalidades principales
1. Registrar recibos de CFE manualmente, validando fechas y valores.
2. Consultar el historial y comparar consumos e importes entre periodos válidos.
3. Analizar aumentos o disminuciones y mostrar una recomendación general cuando el consumo sea mayor.

## Mejoras del diseño aplicadas
- Validación detallada de campos, fechas y valores antes del guardado; mensajes específicos y advertencia de periodos duplicados o traslapados.
- Comparación con control de traslapes, visualización de la duración de cada periodo y advertencia cuando los periodos tienen distinta duración.
- Casos de aceptación y maquetas complementarias incorporados para revisar los resultados esperados.

Las mejoras se aplicaron a la especificación y a maquetas del prototipo. No se afirma que el sistema esté implementado como una aplicación funcional ni que las mejoras provengan de retroalimentación externa.

## Alcance
- Sin conexión automática con CFE ni lectura de medidores.
- Sin desglosar el consumo por aparato.
- El componente inteligente es una regla de comparación, no un modelo avanzado de IA.
- Prototipo base en PowerPoint de cuatro pantallas, más dos maquetas vectoriales complementarias para los estados revisados.

## Estructura del repositorio
- docs/: índice, problema, requerimientos, objetivos y alcance, componente inteligente, prototipo, validación, pruebas de aceptación, control de versiones, riesgos y planificación.
- docs/diagramas/: cuatro diagramas SVG.
- docs/gestion/: riesgos y tablero de tareas.
- prototipo/: PowerPoint base y maquetas complementarias de las mejoras.
- evidencias/: capturas originales y evidencia de las mejoras.
- entrega/: documento integrador, presentación y guion en Word/PDF/PPTX.

## Enlaces
- [GitHub Projects](https://github.com/users/Encorser/projects/1/views/1)
- [Documento integrador y exposición](entrega/README.md)
- [Bitácora de mejoras aplicadas](evidencias/mejoras-aplicadas.md)

## Estado de validación
Las dos mejoras de diseño están documentadas. Sigue pendiente obtener retroalimentación real de la docente o de compañeros, confirmar la pertinencia de los cambios y registrar cualquier ajuste derivado. Las listas preliminares no equivalen a una validación formal.
