# Guion de exposición (5 a 7 minutos)

**Proyecto:** Control de consumo energético en una casa habitación  
**Materia:** Gestión de Proyectos de Software

## Diapositiva 1. Presentación (20 segundos)

Buenas tardes. Voy a presentar el proyecto “Control de consumo energético en una casa habitación”, realizado para la materia Gestión de Proyectos de Software. El objetivo fue delimitar una propuesta sencilla, documentar sus requerimientos y preparar un prototipo visual, sin desarrollar una aplicación funcional completa.

## Diapositiva 2. Problema y usuario (35 segundos)

El problema que se plantea es la falta de un registro organizado que permita revisar de forma práctica la evolución del consumo eléctrico y de los importes facturados. El usuario será únicamente una persona de la vivienda. La propuesta reúne la información de los recibos de CFE y facilita compararla, sin conectarse de manera automática con CFE. El lugar y los datos que utilizamos son hipotéticos.

## Diapositiva 3. Objetivos y alcance (40 segundos)

El objetivo general es diseñar un sistema de control del consumo, apoyado en registros manuales. El alcance se mantuvo limitado para cumplir la guía: tres funcionalidades principales, hasta tres grupos de información y cuatro pantallas. No incluye medidores, sensores, integración con CFE, pagos ni identificación del aparato que causó un incremento.

## Diapositiva 4. Requerimientos (40 segundos)

Se definieron tres requerimientos funcionales: registrar recibos, consultar y comparar periodos, y detectar incrementos para mostrar una recomendación. Se agregaron dos requisitos no funcionales de claridad y conservación de datos, y tres grupos de información: recibos, resultados y recomendaciones. El historial se consulta desde los recibos, por lo que no se cuenta como un cuarto grupo.

## Diapositiva 5. Función inteligente (40 segundos)

La función inteligente compara el consumo total del periodo seleccionado con el periodo anterior. Por ejemplo, si el registro anterior es de 285 kWh y el actual de 320, hay una diferencia de 35 kWh, equivalente aproximadamente a 12.3 por ciento. El sistema puede mostrar una recomendación general. Si no hay un recibo anterior, debe decir que no cuenta con información suficiente. Como los periodos pueden durar diferente número de días, comparamos el total registrado, no el consumo diario.

## Diapositiva 6. Prototipo, pantallas 1 y 2 (35 segundos)

El prototipo tiene cuatro pantallas. La primera es un panel principal para ver el último consumo e importe y entrar a las demás funciones. La segunda es el formulario donde se registran manualmente las fechas del recibo, los kilowatt-hora y el importe. Se espera que el sistema avise si faltan datos, aunque la maqueta no ejecuta estas interacciones.

## Diapositiva 7. Prototipo, pantallas 3 y 4 (35 segundos)

La tercera pantalla permite consultar el historial y comparar dos periodos. La cuarta muestra el resultado del análisis. Si el consumo aumentó, aparecerá una recomendación general. Si no hay un periodo anterior, se indica que la comparación no está disponible. Los valores mostrados en el prototipo son hipotéticos.

## Diapositiva 8. Diagramas (35 segundos)

El diagrama de casos de uso muestra un solo actor y las tres funciones principales con algunas acciones auxiliares. El diagrama de actividades muestra el proceso desde la captura y validación del recibo, hasta la comparación y la presentación de resultados. También se consideran las alternativas de datos inválidos o falta de un periodo anterior.

## Diapositiva 9. Arquitectura y datos (35 segundos)

La arquitectura se representa en cuatro capas: presentación, aplicación, negocio y acceso a datos. Es una propuesta conceptual, no un sistema ya implementado. El DFD de nivel 1 destaca al usuario, los tres procesos principales y los tres grupos de información. Se conserva el alcance de un solo tipo de usuario y sin integración externa con CFE.

## Diapositiva 10. Gestión, riesgos y GitHub (40 segundos)

La gestión se organizó en ocho tareas, dentro del límite marcado en la guía. Se registraron tres riesgos: captura incorrecta, falta de recibos para comparar y retrasos en la documentación. Se plantearon acciones de prevención para cada uno. En GitHub ya se encuentran el README, los documentos, los diagramas en SVG, el PowerPoint y seis capturas del propio repositorio.

## Diapositiva 11. Conclusión (35 segundos)

En conclusión, tenemos una propuesta acotada, sus requerimientos, diagramas, prototipo y la organización del trabajo en GitHub. La función inteligente es sencilla y se basa en los datos disponibles. La validación aún no se ha realizado formalmente; por eso falta presentar el prototipo al grupo y a la docente, recoger sus comentarios y aplicar al menos dos mejoras antes de la entrega definitiva. Muchas gracias.