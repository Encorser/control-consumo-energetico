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
- `docs/`: [índice de la documentación](docs/README.md), planteamiento, requerimientos, objetivos y alcance, componente inteligente, prototipo, control de versiones, gestión de riesgos y [guion de exposición](docs/guion-exposicion.md).
- `docs/diagramas/`: los [cuatro diagramas en formato SVG](docs/diagramas/README.md).
- `docs/gestion/`: riesgos y tablero de tareas.
- `prototipo/`: [PowerPoint de cuatro pantallas](prototipo/(Presentacion)%20prototipo_control_consumo_energetico.pptx).
- `evidencias/`: [seis capturas del proyecto actual](evidencias/README.md) y referencia de una actividad previa identificada por separado.
- `entrega/`: [índice y lista de archivos finales](entrega/README.md). El documento integrador y la exposición están preparados como archivos descargables; sus binarios aún deben cargarse aquí desde GitHub.

## Tablero de gestión
[GitHub Projects](https://github.com/users/Encorser/projects/1/views/1)

## Nota académica
El escenario y los datos de ejemplo del prototipo son hipotéticos. El sistema no consulta ni modifica información real de CFE. La validación formal sigue pendiente de la revisión real del grupo y la docente; sus comentarios y las dos mejoras posteriores no se simulan ni se inventan.
