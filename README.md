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
- El prototipo visual se prepara en PowerPoint y consta de cuatro pantallas: panel principal, registro, historial/comparación y análisis/recomendaciones.

## Estructura del repositorio
- `docs/`: documentación del proyecto, requerimientos, diagramas y gestión.
- `prototipo/`: prototipo visual de PowerPoint y materiales relacionados.
- `evidencias/`: capturas del tablero, historial de commits, revisiones y validación.

## Tablero de gestión
Tablero GitHub Projects: https://github.com/users/Encorser/projects/1/views/1

La lista de tareas se documenta en [docs/gestion/tablero-tareas.md](docs/gestion/tablero-tareas.md). Las tareas se administran mediante incidencias asociadas a este repositorio.

## Nota académica
El escenario y los datos de ejemplo del prototipo son hipotéticos. El sistema no consulta ni modifica información real de CFE.
