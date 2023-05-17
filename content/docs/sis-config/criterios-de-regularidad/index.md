---
title: "Crear Criterios de Regularidad"
lead: "Los Criterios de regularidad establecen los parámetros que se utilizarán para determinar la condición o Estado en el que están los estudiantes en relación al cursado y aprobación de la materia."
date: 2022-09-23T11:17:02-0300
lastmod: 2020-11-16T13:59:39+01:00
draft: false
images: []
weight: 150
toc: true
---
Un criterio de regularidad es un conjunto de condiciones que se aplican sobre diferentes tipos de evaluaciones tales como Trabajos Prácticos (TPs) o parciales y sobre la Asistencia (porcentaje permitido de ausentes) que al cumplirse (o al no cumplirse) determina el Estado académico final (regular, libre por nota, libre por inasistencia) de un estudiante en una materia.

Los Criterios de regularidad son los siguientes y deben establecerse en un cierto orden para cada **Tipo de materia**: MIA, MEC, de Proceso, etc.

- **Promoción directa** (el estudiante ha obtenido notas que lo eximen de rendir un examen final)
- **Promoción indirecta** (el estudiante ha obtenido notas que lo eximen de rendir un examen final)
- **Regular** (el estudiante ha obtenido notas en los exámenes parciales que no lo eximen de rendir un examen final)
- **Libre por nota** (el estudiante se ha quedado libre por aplazo)
- **Libre por asistencia** (el estudiante se ha quedado libre por inasistencias)

Configurar un **Criterio de Regularidad** significa tomar, por ejemplo, una materia **MEC** y establecer de acuerdo a ciertos parámetros en qué condición de regularidad está el estudiante en relación a la materia. Las fórmulas relacionadas con obtener una calificación o nota mayor o menor a un número dado, por ejemplo, **MEC** / **Nota de TPA mayor a 7**, o con respecto a un porcentaje de asistencia, por ejemplo, **MEC** / **Asistencia 75%**, se configuran previamente en un **Grupo de Evaluaciones y Expresiones**.

De este modo, si la universidad decidiera que para una materia **MEC** los **TRABAJOS PRÁCTICOS ADICIONALES (TPA)** deben tener una nota **mayor a 7** para promocionar la materia, es decir para no tener que rendir examen final (Criterio de Regularidad), se deberá especificar en un **Criterio de Regularidad** cuya configuración sería: **MEC**, **PROMOCIÓN DIRECTA**, **Nota de TPA > 7**

{{<warning text="Para el <b>Criterio de regularidad</b> de este ejemplo, el <b>Grupo de Evaluaciones y Expresiones</b> que indica que para Materias MEC la <b>Nota de TPA > 7</b> debe haberse establecido anteriormente.">}}
<br>
1. Asegúrate de estar conectado a la red de Siglo 21 o a la VPN y luego ingresa al **Sistema de Configuraciones Académicas** también llamado **SIS Config** con las mismas credenciales que utilizas para entrar al SGU. Por defecto, se desplegará el Módulo ** de estudio**.
2. Haz clic en el Módulo **Criterios de regularidad**. Por defecto, se desplegará el primer criterio de la lista de criterios ya establecidos.
   
   Si recorremos la lista de la columna **Criterios de regularidad** podremos ver otros criterios en donde se especifica qué debe suceder para que la condición o **Estado** de una materia sea de **Promoción directa**, **Promoción indirecta**, **Regular**, **Libre por nota**, o **Libre por asistencia**.

A continuación se procederá a la creación del **Criterio de Regularidad** llamado **PROCESO – PRESENCIAL 2023** para mostrar todo el proceso desde su inicio.

3. Haz clic en el botón **MODO EDICIÓN** y luego en el signo **+**.
4. A continuación, ingresa un nombre para el **Criterio de regularidad** que estás por configurar. Este nombre debe incluir:
   - el tipo de materia: EFIP, MEC, MIA, De Proceso, etc.
   - la modalidad: Presencial, Sin asistencia, etc.

A modo de ejemplo, ingresa el nombre **PROCESO – PRESENCIAL**, y luego se desliza el botón desplegable **Ejecutar al inicio del período** si el **Criterio de Regularidad** que se está creando se debe aplicar al inicio de un Período.

5. Haz clic en el botón **Guardar**. El **Nombre** del nuevo criterio será agregado en el sector izquierdo de la pantalla, al final de la lista.
6. Posiciónate en el nuevo criterio agregado y haz clic en **MODO EDICIÓN**.
7. En la ventana que se despliega, haz clic en **AGREGAR GRUPO DE EVALUACIÓN**.
8. En la ventana que se despliega, selecciona un ítem de evaluación – Parciales, TPs, TPAs, o un ítem de Asistencia.
9. Haz clic en el botón **Confirmar**. El **Grupo de Evaluación** recién agregado se desplegará en la pantalla.

{{<note text="Este grupo de evaluación ya debe haber sido creado en el Módulo <b>Grupo de Evaluaciones y Expresiones</b> del <b>SIS Config</b>.">}}
<br>

10. Haz clic en **Agregar tipo**. Esto definirá como se utilizará la **Expresión** (FÓRMULA) establecida en el **Grupo de evaluación y expresión** seleccionado.
11. En **Agregar tipo**, selecciona **Aprobación**. A continuación, se despliega la ventana **Aprobación**, en donde deberás completar:
    - el **Nombre** que definirá la condición de regularidad: **Promoción directa**, **Promoción Indirecta**
    - la **Expresión**, la cual se debe haber establecido en un **Grupo de Evaluaciones y Expresiones** para el ítem evaluador (puede haber más de una Expresión dentro del **Grupo de Evaluaciones y Expresiones** para el ítem evaluador)
    - el **Estado** de la materia, el cual es el Estado que tendrá la materia de acuerdo al criterio de regularidad que se está creando o definiendo.

12.  Una vez completados los campos de la ventana **Aprobación**, haz clic en el botón **CONFIRMAR**. A continuación, se desplegará una ventana en donde podemos observar que para una materia del tipo **Proceso**, cuya modalidad es **Presencial**, hasta ahora hemos establecido que la condición o Estado será de **Promoción Directa** con respecto a un ítem de evaluación dado.
13. Selecciona la **Condición**. En este ejemplo, **Sin final** es la única opción disponible porque el **Criterio de Regularidad** es **_Promoción Directa_**.
14. Haz clic en **Agregar Grupo de Evaluación** nuevamente para agregar otro ítem de evaluación que se corresponda con el **Criterio de Regularidad**: **_Promoción Directa_**.

A modo de ejemplo, selecciona **Trabajos Prácticos (TPs)**.

15. Haz clic en el botón **Confirmar**. El **Grupo de Evaluación** recién agregado se desplegará en la pantalla, debajo del primer **Grupo de Evaluación**.
16. Para terminar de definir el **Criterio de regularidad** con respecto a los Trabajos Prácticos, debes establecer una **Condición**. Haz clic en la lista desplegable, y selecciona una condición.
17. Haz clic en **Agregar Grupo de Evaluación** nuevamente para agregar un ítem de asistencia que se corresponda con el **Criterio de Regularidad**: **_Promoción Directa_**.
18. Una vez seleccionado el **Grupo de Evaluación**: **_Asistencia_**, haz clic en el botón **Confirmar**.
19. Para terminar de definir el **Criterio de regularidad** con respecto a la **Asistencia**, debes establecer una **Condición**. Haz clic en la lista desplegable, y selecciona una condición.

Para el **Criterio de regularidad**: **_Promoción Directa_**, la universidad puede fijar condiciones para la asistencia o no. Dependiendo de los estándares que desee fijar, podrá optar por fijar un **75% de asistencia a módulos** o por no fijar ninguna restricción al respecto.

{{<note text="Al criterio de regularidad <b>Promoción directa</b> se le pueden agregar más <b>Grupos de Evaluación</b> tales como <b>Parciales</b> o <b>Correlativas</b> para así establecer más condiciones para que los estudiantes obtengan la condición o Estado de <b>Promoción directa</b> para un tipo de materia dada.">}}
<br>

20. Para crear el siguiente **Criterio de Regularidad** para el mismo **Tipo de materia** + **Modalidad:** **_Proceso – Presencial_**, haz clic en **Agregar tipo**, selecciona **Aprobación**, y en **Nombre**, coloca **_Promoción Indirecta_**.
21. Selecciona una de las opciones del campo **Expresión**. En este ejemplo, se seleccionará **Examen final con 4 o más**.
22. Selecciona el **Estado** de la materia, el cual es el Estado que tendrá la materia de acuerdo al criterio de regularidad que se está creando o definiendo.
23. Haz clic en el botón **Confirmar**. A continuación, verás el nuevo criterio desplegado a la derecha del de **Promoción directa**.
24. Agrega las condiciones para los ítems de evaluación y asistencia que ya ingresaste para **Promoción directa**.
   
#### Ejemplo al “Agregar tipo” igual a “Requiere Examen”
25. Para crear el siguiente **Criterio de Regularidad** para el mismo tipo de materia + Modalidad: **Proceso – Presencial**, haz clic en **Agregar tipo**, pero esta vez, en vez de **_Aprobación_**, selecciona **_Requiere examen_**.
26. Selecciona el **Nombre:** **_Regular_**, y las opciones restantes teniendo en cuenta que el Estado que se está configurando es el de **Regular** y luego haz clic en el botón **Confirmar**. A continuación, se desplegará el nuevo **Estado** a la derecha de los otros ya creados.
27. Agrega las condiciones para los ítems de evaluación y asistencia que ya ingresaste para **Promoción directa** y de ser necesario, agrega un ítem de evaluación adicional, por ejemplo, **Correlativas**.
28. Haz clic en el botón **Guardar** y confirma los cambios.

#### Ejemplo al “Agregar tipo” igual a “Desaprobación”
29. Haz clic nuevamente en **Agregar tipo** y selecciona **Desaprobación**. A continuación, se desplegará la ventana **Desaprobación**.
30. En la ventana **Desaprobación**, completa el **Nombre** que definirá que sucederá si el estudiante no aprueba cualquier tipo de evaluación. Es decir, la condición o **_Estado_** en la que quedará el estudiante en relación a una materia de un tipo determinado si es aplazado en los exámenes con los que la universidad evalúa su desempeño – o si su asistencia no alcanza al nivel establecido por la universidad: **Libre por nota** y **Libre por inasistencia**. Ingresa, por ejemplo, **Libre por Nota**.
31. Una vez completados los campos de la ventana **Desaprobación**, haz clic en el botón **CONFIRMAR**. A continuación, verás el **Estado** **_Libre por Nota_** a la derecha del último Estado configurado.
32. Agrega las condiciones por **Grupo de evaluación** (Asistencia, Trabajos Prácticos, Finales, Parciales).
33. Haz clic nuevamente en **Agregar tipo** y vuele a seleccionar **Desaprobación**, pero esta vez en vez de crear el **Estado** **_Libre por Nota_**, establece el Estado **_Libre por Asistencia_**.
34. Una vez completados los campos de la ventana **Desaprobación**, haz clic en el botón **CONFIRMAR**. A continuación, verás el **Estado** **_Libre por Asistencia_** a la derecha del último Estado configurado.
35. Agrega las condiciones por **Grupo de evaluación** (Asistencia, Trabajos Prácticos, Finales, Parciales).
36. Realiza el mismo procedimiento para otros tipos de **materias + modalidad**. Recuerda que al crear un **Criterio de Regularidad** debes contar con:

 - **Niveles de Estudio** en donde se asocian **Nivel de Estudio** + **Modalidad** + **Turno de cursado** y **Grupos de Seguridad**
 - **Evaluaciones y Expresiones** que establecen:
   - Una configuración que indica que para un **ítem evaluador** (Trabajos Prácticos (TPs), Parciales, Actividades Prácticas Integradoras (APIs), etc.) hay una **FÓRMULA** (“expresión”) que puede combinar, entre otros ítems, Notas + % de Asistencia
   - y una configuración que establece el **porcentaje de Asistencia** que un estudiante debe tener para poder promocionar la materia

## Véase también

[Niveles de Estudio →]({{< relref "/nivel-de-estudio" >}} "Niveles de Estudio")

[Evaluaciones y Expresiones →]({{< relref "/evaluaciones-y-expresiones" >}} "Evaluaciones y Expresiones")