---
title: "Crear Evaluaciones y Expresiones"
lead: "Determina el Estado en la que se encuentra un estudiante en relación a la promoción de las materias que cursa. Para ello, crea un Grupo de Evaluaciones y Expresiones y establece una configuración para una ítem de evaluación y una configuración para la la asistencia."
date: 2022-09-23T11:17:02-0300
lastmod: 2020-11-16T13:59:39+01:00
draft: false
images: []
weight: 150
toc: true
---

**Grupo de Evaluaciones y Expresiones de un ítem de evaluación:** Esta es una configuración que establece que para un ítem evaluador (Trabajos Prácticos (TPs), Parciales, Finales, Actividades Prácticas Integradoras (APIs), etc.) haya una FÓRMULA (“expresión”) que puede combinar, entre otros ítems, Notas + % de Asistencia, para que luego al configurar un **Criterio de Regularidad** se establezca que el Estado del estudiante sea "regular", “promoción”, “libre”, etc.

**Grupo de Evaluaciones y Expresiones de la asistencia:** Esta configuración establece que, por ejemplo, para la Asistencia en la modalidad Presencial haya una FÓRMULA (“expresión”) que indique cuál debe ser el porcentaje de módulos a una materia a los que los estudiantes deben concurrir para que luego el Módulo **Criterios de Regularidad** lo utilice en sus propias fórmulas.

#### Crear “Grupos de Evaluaciones y Expresiones” para un Ítem Evaluador

Cuando se agrega un **Grupo de Evaluaciones y Expresiones** primero se agrega el ítem evaluador, por ejemplo, Finales, y luego la **Expresión** (FÓRMULA).

1. Asegúrate de estar conectado a la red de Siglo 21 o a la VPN y luego ingresa al **Sistema de Configuraciones Académicas** también llamado **SIS Config** con las mismas credenciales que utilizas para entrar al SGU. Por defecto, se desplegará el Módulo **Nivel de estudio**.
2. Haz clic en el Módulo **Evaluaciones y expresiones**. Por defecto, se desplegarán la o las instancias de evaluación y expresión ya establecidas del primer ítem evaluador o de Asistencia listado a la izquierda de la pantalla.
3. Para agregar un ítem de evaluación (TP, Parciales, etc.), haz clic en el botón **MODO EDICIÓN** para habilitar el botón que te permitirá añadir un nuevo **Grupo de Evaluaciones y Expresiones**. Recuerda que debes comenzar por añadir un ítem evaluador o de asistencia.
4. Haz clic en el botón verde con el signo **+** para desplegar la ventana **Crear grupo de evaluaciones y expresiones** – y agrega un Nombre para el grupo (puede ser el mismo nombre del ítem evaluador, por ejemplo, “PARCIALES”).
5. Haz clic en el botón **Guardar**. A continuación, verás desplegado el nombre del grupo (siguiendo con el mismo ejemplo, “PARCIALES”) en el panel izquierdo de la pantalla.
6. Haz clic en el nuevo grupo creado para desplegar la pantalla que tendrá el nombre del ítem de evaluación (por ejemplo, “PARCIALES”) y las solapas “EVALUACIONES” y “EXPRESIONES”.
7. Haz clic en el botón **+** para agregar una **EVALUACIÓN**.
8. A continuación, se habilitarán los campos para la pestaña **Evaluaciones** donde debes ingresar:
   - un **Nombre interno** (no visible para los estudiantes): Nombre con el que se identificará la **Evaluación** (el ítem de evaluación o de asistencia) de este **Grupo de Evaluaciones y Expresiones**. Puede ser igual al ítem agregado (“PARCIALES”), o un poco más descriptivo.
   - un **Nombre externo** (visible para los estudiantes): Puede ser igual al **Nombre interno** o más descriptivo  - o menos formal. Es el Nombre con el que los estudiantes verán la **Evaluación**. Por ejemplo, **Parcial 20 preguntas**
   - un **Código** que identifique el ítem de evaluación, por ejemplo, **FFF**
   - la **Fuente**: se refiere a si se está agregando un **ítem de evaluación** como lo es un examen, o si se está agregando una actividad o una **Asistencia**.
   - un **Tipo**: Se desplegará de acuerdo a la **Fuente** seleccionada.
   - un **Objetivo**: En ítem evaluador **Parciales** y **TPs**, el **Objetivo** hace referencia a los ID en Base de Datos de cada uno de estos. Por ejemplo, en Primer Parcial, el Objetivo es igual a 19, que es el ID de la tabla “ue_tipos_examenes”. Esto sirve para evaluar la expresión posteriormente y buscar, en base de datos, la nota correspondiente. En **TPs**, el Objetivo es 1, 2, 3, 4 según el número de TP. En otros ítems evaluadores, solo es un valor numérico sin significado.

9. Dirígete a la pestaña **Expresiones** y haz clic en el botón **+**. A continuación, se desplegará la pantalla donde debes ingresar la **Expresión** o FÓRMULA para terminar de configurar el **Grupo de Evaluaciones y Expresiones** cuyo nombre es el del ítem de evaluación (por ejemplo, “PARCIALES”).
10. En esta pantalla deberás completar:
    - un **Nombre interno** (no visible para los estudiantes): Nombre con el que el Usuario (co-docente) identificará la **Expresión** (FÓRMULA)
    - un **Nombre externo** (visible para los estudiantes): Nombre con el que los estudiantes verán la **Expresión** (FÓRMULA)
    - el Tipo de expresión que identifique si la FÓRMULA será utilizada para un **Cálculo de estado**, un **Cálculo de nota de aprobación** o una combinación de notas y cálculo de estado.
    - la **Expresión** o FÓRMULA que especifique un cálculo que luego será utilizado por un **Criterio de Regularidad** que determinará que si la calificación (o asistencia) del estudiante se ajusta o coincide con la FÓRMULA del ítem evaluador (en este ejemplo, con qué calificación o nota se aprueba un examen final), su condición de regularidad frente a una materia será de “regular”, “promoción”, “no promoción”, o “libre”. Por ejemplo: **FFF > 4**.

11. Haz clic en el botón **Guardar** y luego confirma que quieres realizar los cambios. A continuación, se desplegará un mensaje informando que **_El grupo de evaluaciones y expresiones se creó con éxito_** y verás el grupo **Evaluación + Expresión** (por ejemplo, “PARCIALES”) listado en el sector izquierdo de la pantalla.

A modo de ejemplo, se ha creado entonces un **Grupo de Evaluaciones y Expresiones** para un ítem evaluador llamado **PARCIALES** cuyo **Código** es **FFF** con una **Expresión** o FÓRMULA que simplemente dice: **FFF > 4**. Es decir, aún no se establece qué sucede si el estudiante obtiene una nota mayor a 4 con este **Grupo de Evaluaciones y Expresiones**.

{{<note text="Para indicar qué sucede cuando un estudiante obtiene una calificación o nota mayor a 4 en un examen parcial, se debe crear un <b>Criterio de Regularidad</b> que lo determine. Para ello, ver el <b>Módulo Criterios de regularidad</b>.">}}

12. Verifica que el **Grupo de Evaluaciones y Expresiones** llamado **PARCIALES** contenga la información que ingresaste al crearlo. Para ello, haz clic en **PARCIALES** en el sector izquierdo de la pantalla y luego en las pestañas **Evaluaciones** y **Expresiones** para verificar su contenido.

#### Crear “Grupos de Evaluaciones y Expresiones” para una Asistencia

{{<note text="Cuando se agrega un <b>Grupo de Evaluaciones y Expresiones</b> primero se agrega el tipo de Asistencia, por ejemplo, <b>Presencial</b>, y luego la <b>Expresión</b> (FÓRMULA).">}}

13. Asegúrate de estar conectado a la red de Siglo 21 o a la VPN y luego ingresa al **Sistema de Configuraciones Académicas** también llamado **SIS Config** con las mismas credenciales que utilizas para entrar al SGU. Por defecto, se desplegará el Módulo **Nivel de estudio**.
14. Haz clic en el Módulo **Evaluaciones y expresiones**. Por defecto, se desplegarán la o las instancias de evaluación y expresión ya establecidas del primer ítem de evaluación o de Asistencia listado a la izquierda de la pantalla.
15. Haz clic en el botón **MODO EDICIÓN** para habilitar el botón que te permitirá añadir un nuevo **Grupo de Evaluaciones y Expresiones**. Recuerda que debes comenzar por añadir un tipo de **ASISTENCIA**.
16. Haz clic en el botón verde con el signo **+** para desplegar la ventana **Crear grupo de evaluaciones y expresiones** – y agrega un Nombre para el grupo (es el nombre del tipo de asistencia, por ejemplo, **ASISTENCIA HÍBRIDA**).
17. Haz clic en el botón **Guardar**. A continuación, verás desplegada la asistencia recién agregada (en este ejemplo, **ASISTENCIA HÍBRIDA**) en el sector izquierdo de la pantalla.
18. Haz clic en el nuevo grupo creado – en **ASISTENCIA HÍBRIDA**, ubicado en el sector izquierdo de la pantalla para desplegar la pantalla **ASISTENCIA HÍBRIDA** con las solapas **EVALUACIONES** y **EXPRESIONES**.
19. Para agregar una **EVALUACIÓN**, haz clic en el botón **+**. A continuación, se habilitarán los campos para la pestaña **Evaluaciones** donde debes ingresar:
    - un **Nombre interno** (no visible para los estudiantes): Nombre con el que el Usuario (co-docente) identificará la **Evaluación** (el ítem de evaluación o de asistencia) de este **Grupo de Evaluaciones y Expresiones**. Puede ser igual al ítem agregado (en este ejemplo, **Asistencia Híbrida**), o un poco más descriptivo, por ejemplo, **_Número de Asistencias a Clases Híbridas_**
    - un **Nombre externo** (visible para los estudiantes): Puede ser igual al **Nombre interno** o más descriptivo  - o menos formal. Es el Nombre con el que los estudiantes verán la **Evaluación**. Por ejemplo, **_Número de Asistencias_**
    - un **Código** que identifique la evaluación, por ejemplo, CCHT (Cantidad Clases Híbridas Teleclases)
    - la **Fuente**: se refiere a si se está agregando un ítem evaluador, una actividad o una Asistencia.
    - el **Tipo**: aquí se desplegarán las opciones de acuerdo a la **Fuente** seleccionada. Como se está configurando una **Asistencia**, el **Tipo** será el número de módulos presenciales o virtuales a los que los estudiantes deberán asistir o el mayor número de ausentes que podrán tener en una u otra modalidad.

20. Dirígete a la pestaña **Expresiones** y haz clic en el botón **+**. A continuación, se desplegará la pantalla donde debes ingresar la **Expresión** (FÓRMULA) para terminar de configurar la **Evaluación y Expresión** ingresada (en este ejemplo, **Asistencia Híbrida**). En esta pantalla deberás completar:
    - un **Nombre interno** (no visible para los estudiantes): Un nombre que indique el porcentaje de asistencias que se requiere para la porción de teleclases de las Clases Híbridas, por ejemplo, **_75% Asistencia_**.
    - un **Nombre externo** (visible para los estudiantes): El mismo Porcentaje de Asistencias un poco más descriptivo. Por ejemplo **_75% de Asistencia a Teleclases_**.
    - el **Tipo** de expresión que identifique si la FÓRMULA será utilizada para un **Cálculo de estado**, un **Cálculo de nota de aprobación** o una combinación de notas y cálculo de estado según la asistencia del estudiante.
    - la **Expresión** (FÓRMULA) que especifique cómo se realiza el cálculo, según el **Tipo de expresión** establecido, que luego será utilizado por un **Criterio de Regularidad** que determinará según el resultado que arroje la fórmula en relación a la asistencia del estudiante su condición de regularidad frente a una materia dada.

21. Por último, haz clic en el botón **Guardar**. A continuación, se desplegará un mensaje informando que el grupo de evaluaciones y expresiones se creó con éxito y verás la **Evaluación + Expresión** que en este ejemplo es **ASISTENCIA HÍBRIDA** listada en el sector izquierdo de la pantalla.

## Véase también

[Niveles de Estudio →]({{< relref "/nivel-de-estudio" >}} "Niveles de Estudio")

[Criterios de Regularidad →]({{< relref "/criterios-de-regularidad" >}} "Criterios de Regularidad")