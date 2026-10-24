# 4. Prototipo

**Estado:** prototipo base de cuatro pantallas incorporado en PowerPoint; dos detalles de interfaz se ampliaron mediante maquetas vectoriales complementarias para documentar las mejoras de validación de entrada y comparación de periodos.

**Archivo base:** [PowerPoint de cuatro pantallas](../prototipo/%28Presentacion%29%20prototipo_control_consumo_energetico.pptx).

**Maquetas complementarias revisadas:**
- [Registro de recibo con validaciones](../prototipo/mejoras/registro-validado.svg).
- [Historial y comparación con advertencia de duración](../prototipo/mejoras/comparacion-periodos.svg).

Las maquetas SVG representan el diseño propuesto de estados y mensajes; no son capturas de una aplicación funcional ni sustituyen el archivo PowerPoint original. Las cifras son hipotéticas.

## Pantalla 1. Panel principal
**Objetivo:** resumir el consumo registrado y facilitar el acceso a las funciones del sistema.

**Elementos:** último periodo disponible, consumo e importe y accesos a registro, historial y análisis. Si faltan datos, el panel deberá indicarlo sin inventar cifras.

## Pantalla 2. Registro de recibo de CFE
**Objetivo:** permitir la captura manual y evitar guardar datos incompletos o inválidos.

**Campos:** fecha inicial y final del periodo, consumo en kWh e importe en MXN.

**Validaciones incorporadas en la propuesta de diseño:**
- Fecha inicial igual o anterior a la fecha final.
- Consumo e importe numéricos y no negativos.
- Campos obligatorios completos.
- Advertencia ante periodos que coincidan o se traslapen con un registro existente.
- Mensaje asociado al campo que necesita corrección; el guardado queda bloqueado hasta corregir los errores.

## Pantalla 3. Historial y comparación
**Objetivo:** consultar recibos y comparar periodos válidos.

**Elementos:** fechas, duración, consumo e importe por periodo, diferencias y selección de periodos.

**Reglas incorporadas en la propuesta de diseño:** no comparar rangos que se traslapen; informar cuando no existan dos periodos válidos; mostrar una advertencia visible si las duraciones difieren. Los resultados siguen siendo consumos totales por periodo y no se denominan consumo diario.

## Pantalla 4. Análisis y recomendaciones
**Objetivo:** exponer el resultado de la función basada en reglas.

**Elementos:** periodos comparados, consumos, diferencia, estado de variación y recomendación cuando corresponda.

**Interacción:** si una comparación válida indica mayor consumo, se muestra una recomendación general. Si el consumo bajó o permaneció igual, se informa el resultado sin activar la recomendación por aumento. Si los datos son insuficientes, no se presenta una conclusión.

## Correspondencia entre artefactos

Las reglas ampliadas se documentan en [requerimientos](requerimientos.md), [componente inteligente](componente-inteligente.md) y [pruebas de aceptación](pruebas-aceptacion.md). La [bitácora de mejoras](../evidencias/mejoras-aplicadas.md) explica los cambios y diferencia el diseño revisado de una validación externa real.

## Límites de la evidencia

Las dos maquetas SVG son evidencia del diseño actualizado. No prueban que las reglas se hayan ejecutado en un sistema funcional ni que la docente o un grupo las hayan aprobado. La validación externa y la incorporación de retroalimentación real siguen pendientes.
