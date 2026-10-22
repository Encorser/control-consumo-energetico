# Control de consumo energético en una casa habitación

Proyecto académico de la materia **Gestión de Proyectos de Software**.

## Descripción
Se propone un sistema para una vivienda familiar hipotética ubicada en Tuzamapan, Xalapa, Veracruz, México. El usuario registrará manualmente los recibos de la Comisión Federal de Electricidad (CFE), incluyendo el periodo facturado, el consumo en kWh y el importe en pesos mexicanos.

## Funcionalidades principales
1. Registrar recibos de CFE manualmente.
2. Consultar y comparar consumos e importes entre periodos.
3. Analizar variaciones del consumo y mostrar recomendaciones generales cuando el consumo actual sea mayor que el anterior.

## Alcance
- No hay conexión automática con CFE ni lectura de medidores.
- No se analiza el consumo individual de cada aparato.
- El componente inteligente utiliza una regla sencilla de comparación; no es un modelo avanzado de IA.
- El prototipo visual está diseñado en PowerPoint y consta de cuatro pantallas: panel principal, registro, historial/comparación y análisis/recomendaciones. El archivo ya está incorporado en la carpeta `prototipo/`.

## Estructura del repositorio
- `docs/`: [índice de la documentación](docs/README.md), [planteamiento del problema](docs/problema-contexto.md), [requerimientos](docs/requerimientos.md), [objetivos y alcance](docs/objetivos-alcance.md), [componente inteligente](docs/componente-inteligente.md), [prototipo](docs/prototipo.md), [control de versiones](docs/control-versiones.md) y [validación preliminar](docs/validacion.md).
- `docs/diagramas/`: los [cuatro diagramas en formato SVG](docs/diagramas/README.md) (casos de uso, flujo de actividades, arquitectura conceptual y DFD nivel 1).
- `docs/gestion/`: [riesgos](docs/gestion/riesgos.md) y [tablero de tareas](docs/gestion/tablero-tareas.md).
- `prototipo/`: [PowerPoint de cuatro pantallas](prototipo/(Presentacion)%20prototipo_control_consumo_energetico.pptx).
- `evidencias/`: [índice de las seis capturas del proyecto actual](evidencias/README.md) y referencia de una actividad previa claramente identificada.

## Tablero de gestión
Tablero GitHub Projects: https://github.com/users/Encorser/projects/1/views/1

La lista de tareas se documenta en [docs/gestion/tablero-tareas.md](docs/gestion/tablero-tareas.md). Las tareas se administran mediante incidencias asociadas a este repositorio.

## Nota académica
El escenario y los datos de ejemplo del prototipo son hipotéticos. El sistema no consulta ni modifica información real de CFE. Las evidencias de una actividad anterior se conservan como referencia y no sustituyen las capturas del proyecto actual.
