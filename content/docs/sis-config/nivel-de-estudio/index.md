---
title: "Configurar Nivel de Estudio"
lead: "Mediante el módulo Nivel del Estudio, los usuarios podrán registrar nuevas combinaciones de Nivel de Estudio, Modalidad de Estudio, Turno de cursado y Grupos de Seguridad."
date: 2022-09-23T11:17:02-0300
lastmod: 2020-11-16T13:59:39+01:00
draft: false
images: []
weight: 150
toc: true
---

Al término de la creación de dicha combinación, se deberá relacionar:

- un **Tipo de materia** (MIA, MEC, de Proceso, etc.) a la nueva combinación. Así, por ejemplo, se podría relacionar una materia MEC con una combinación dada: MEC + Grado + a Distancia + Tutoría bimestral + Grupo de Seguridad.
- un **Criterio de regularidad** (Por ejemplo, “MEC con Asistencia Teleclases - 2023”)
<br>
<br>
1. Asegúrate de estar conectado a la red de Siglo 21 o a la VPN y luego ingresa al **Sistema de Configuraciones Académicas** también llamado **SIS Config** con las mismas credenciales que utilizas para entrar al SGU. Por defecto, se desplegará el **Módulo Nivel de estudio**.
2. En esta primera pantalla, a la izquierda se visualiza la lista **Nivel de Estudio** con el primer ítem seleccionado por defecto. A la derecha de esta lista, se visualizan tres listas desplegables o secciones:
   - Sección **Configuraciones:** Aquí se listan las combinaciones existentes con el ítem seleccionado en la lista **Nivel de Estudio** y se registran las nuevas combinaciones.
   - Sección **Requisitos de visado:** En esta sección, se confecciona la lista de requisitos que se debe repasar para considerar que el estudiante ha completado una materia y no adeuda ninguna documentación o pago. Asimismo, la misma lista de requisitos tendrá un tiempo de vigencia, el cual se denomina **Duración de la vigencia de visado**: 30, 120, 180 días, etc.
   - Sección **Resoluciones requeridas:** Aquí el usuario deberá marcar o activar con un botón deslizable cuáles son las resoluciones que ya han sido expedidas y están vigentes, siendo éstas la Resolución  rectoral, la Resolución ministerial, y el número de Expediente C.O.N.E.A.U.

{{<note text="Estas son las resoluciones que necesitan tener los <b>Planes de Estudio</b>, por lo que su configuración impacta en el <b>Administrador de carreras</b> cuando desde allí se intenta activar un <b>Plan de Estudio</b>.">}}
<br>

**Ejemplo:** Si desde el **Administrador de carreras** se intenta activar un **Plan de Estudio** para una carrera de GRADO y dicho plan no tuviera **_Resolución ministerial_**, y en SIS Config el **Nivel de estudio** GRADO tiene la opción **_Resolución ministerial_** activa, va a arrojar un mensaje de error. Sin embargo, si se intenta activar un **Plan de Estudio** para un CURSO, y en SIS Config no está establecido que requiere **_Resolución ministerial_**,  dicho plan SÍ se va a poder activar desde el **Administrador de carreras** si no cuenta con una resolución de este tipo.

#### SECCIÓN CONFIGURACIONES

3. Selecciona un **Nivel de Estudio** de la lista ubicada a la izquierda de la pantalla -por ejemplo, **Extragrado**. A continuación, se mostrará cómo asociarlo o combinarlo a una **Modalidad de Estudio**, a un **Turno de cursado**, y a un **Grupo de Seguridad**.
4. En la pantalla principal, se observan 3 listas: **_Configuraciones_**, **_Requisitos de visado_**, y **_Resoluciones Requeridas_**. Haz clic en **Configuraciones**.
5. Haz clic en el botón **Modo Edición**. A continuación, se habitará el botón desplegable **Sedes** lo que te permitirá asociarle a este **Nivel de Estudio** que hemos seleccionado como ejemplo, es decir, **Extragrado**, una **Modalidad de Estudio**, por ejemplo, **_Presencial (P)_** para un **Turno de cursado** que podría ser, por ejemplo, **_Diplomaturas Extragrado_**.
6. Selecciona una **Sede** para indicar la **_Modalidad de Estudio_** (presencial o virtual).
7. Selecciona la **_Submodalidad_** (**_Presencial (P)_**” (a veces indicada como “Presencial .”),  **Presencial Home (PH)**, **Educación Distribuida (ED)** y **Educación Distribuida Home (EDH)**).
8. Selecciona el **Tipo de cursado**.

{{<note text="Así como se puede seleccionar más de una Submodalidad para cada Sede-Modalidad seleccionada, también se podrá seleccionar más de un <b>Tipo de cursado</b> para cada asociación de <b>Niveles de Estudio</b> y </b>Modalidad de Estudio”.</b>.">}}

9. Selecciona el **Grupo de Seguridad**.
10. Haz clic en el botón **Guardar** y luego confirma los cambios.
11. Luego de confirmar los cambios el **SIS Config** te informará que el **Nivel de Estudio** se actualizó con éxito.
12. Cerciórate de que la nueva combinación de **Nivel de Estudio**,  **Modalidad de Estudio**, **Turno de cursado** y **Grupo de seguridad** se haya añadido.

##### Relacionar un Nivel de Estudio con un “Tipo de materia” y un “Criterio de Regularidad”
Recuerda que luego de haber definido una combinación de **Nivel de Estudio** + **Modalidad de Estudio** + **Turno de cursado** + **Grupos de Seguridad**, a continuación deberás asociar un **Tipo de materia** (MEC, MIA, de Proceso, etc.) y un **Criterio de regularidad** a la combinación creada.

13. Si saliste del **Sistema de Configuraciones Académicas** o **SIS Config**, vuelve a asegurarte de estar conectado a la red de Siglo 21 o a la VPN y vuelve a ingresar al SIS Config con las mismas credenciales que utilizas para entrar al SGU. Por defecto, se desplegará el Módulo **Nivel de estudio**.
14. En la lista **Nivel de Estudio** que se encuentra a la izquierda de la pantalla, localiza el **Nivel de Estudio** con el que debas relacionar un **Tipo de materia** determinado. Por ejemplo, localiza el **Nivel de Estudio** **_Extragrado_** para relacionarlo con el **Tipo de materia** MEC.
15. Haz clic en la opción desplegable **Configuraciones**.
16. Haz clic en el botón **MODO EDICIÓN**.
17. A continuación, haz clic en el ícono **Asociar tipos de materia** que se encuentra debajo del **Turno de cursado**.

En la ventana que se despliega, podrás observar si ya existe un **Tipo de materia** o no ya asociado al **Nivel de Estudio** que seleccionaste, por ejemplo, Extragrado y podrás modificar la asociación existente o eliminarla, o agregar una asociación nueva.

18. Para agregar una asociación, haz clic en el botón **MODO EDICIÓN**. A continuación, verás la misma pantalla pero con los botones **GUARDAR** y **CANCELAR** desplegados.
19. Haz clic en el signo **+** que se encuentra en el sector inferior de la pantalla.
20. A continuación, se habilitarán dos listas desplegables: **Tipo de materia** y **Criterio**.
21. Haz clic en la lista desplegable **Tipo de materia** y selecciona una de las opciones que se despliegan -por ejemplo, podrás seleccionar el **Tipo de materia** MEC.
22. Haz clic en la lista desplegable **Criterio** y selecciona una de las opciones que se despliegan. Por ejemplo, selecciona el **Criterio de regularidad**: **_MEC CON ASISTENCIA TELECLASES – 2023_**.
23. Haz clic en el botón **GUARDAR** y verifica que deseas realizar estos cambios.

A continuación, la app **SIS Config** desplegará el mensaje **_Los criterios de regularidad se han asociado de forma correcta_**.

En este ejemplo, hemos entonces asociado al **Nivel de Estudio** Extragrado con sus combinaciones de **Modalidad de Estudio**, **Turno de cursado**, y **Grupo de seguridad** a un **Tipo de materia** MEC y a un **Criterio de regularidad** llamado **_MEC CON ASISTENCIA TELECLASES – 2023_** que ya estaba establecido con anterioridad y que será el responsable de determinar la condición o Estado de una materia MEC para un estudiante que curse una materia Extragrado con las características mencionadas.

#### SECCIÓN REQUISITOS DE VISADO
El visado consiste en verificar por parte de la universidad una serie de requisitos que los estudiantes deben cumplir ya sea de carácter administrativo (el pago de un ticket), en relación a la biblioteca (material prestado y adeudado), o a la documentación que se debe presentar (foto del DNI, Certificado Analítico, etc.).

En esta sección, se establece para cada **Nivel de estudio** los requisitos a nivel Administrativo y en relación a la Biblioteca y a la Documentación a presentar que los estudiantes deben cumplir para que el visado sea satisfactorio.

24. Una vez que se haya añadido una nueva combinación de **Nivel de Estudio**,  **Modalidad de Estudio**, **Turno de cursado** y **Grupo de seguridad**, procede a establecer cuáles son los **Requisitos de Visado** para dicha combinación. Para ello, primero selecciona un **Nivel de estudio** del sector izquierdo de la pantalla, y luego haz clic en el botón **MODO EDICIÓN**. A modo de ejemplo, selecciona el **Nivel de Estudio** **_Extragrado_**.
25. Haz clic en la lista desplegable **Requisitos de visado** para desplegar la sección.

A continuación verás que la sección consta de dos campos: uno en donde se lee **Duración de la vigencia de visado**, el cual establece por cuánto tiempo el visado será válido y por lo que al término de dicho lapso de tiempo la universidad podría volver a requerir una acción por parte del estudiante, y el campo **Nueva documentación**, que como su nombre lo indica, especificará qué documento, copia o certificado el estudiante necesita presentar.

26. En el campo donde se lee **Duración de la vigencia de visado** establece, en números, el tiempo de vigencia del visado, por ejemplo, 180 (días).
27. Haz clic en el signo **+** ubicado en el extremo derecho del campo **Nueva documentación** y luego agrega la documentación que los estudiantes deban presentar para el **Nivel de estudio** seleccionado.

{{<note text="De ser necesario, agrega cualquier otro tipo de documentación que los estudiantes deban presentar para el <b>Nivel de estudio</b> seleccionado.">}}

28. Una vez cargados todos los requisitos, haz clic en el botón **Guardar** y luego confirma el cambio que deseas realizar.
29. Verifica que los cambios fueron realizados.

#### SECCIÓN RESOLUCIONES REQUERIDAS
En esta sección, se indicará cuáles son las Resoluciones que se necesitan para activar el **Plan de Estudios** de una **carrera** que se inserta dentro de una combinación de **Nivel de Estudio** en particular. Las resoluciones existentes son: la Resolución Ministerial, la Resolución Rectoral, y el Expediente C.O.N.E.A.U.

{{<note text="En esta sección, se indica que, si por ejemplo, una carrera se inserta dentro de la combinación </b>Nivel de Estudio</b> Grado; <b>Modalidad de Estudio</b> Presencial (P); <b>Turno de cursado</b> Cuatrimestral; y <b>Grupo de seguridad</b> UE21_ALUMNOS, el <b>Plan de Estudios</b> de dicha carrera sólo podrá activarse desde la app <b>Administrador de Carreras</b> una vez que se emitan la o las Resoluciones Ministerial, Rectoral, o Expediente C.O.N.E.A.U. aquí indicadas.">}}

31. Para activar el **Plan de Estudios** de una carrera que esté comprendida dentro de un **Nivel de Estudio** ya configurado, y una vez ya establecidos los **_Requisitos de Visado_** para dicha combinación, indica cuáles son las **Resoluciones**. Para ello, primero selecciona un **Nivel de estudio** del sector izquierdo de la pantalla, y luego haz clic en el botón **MODO EDICIÓN**.
32. Haz clic en la lista desplegable **Resoluciones requeridas** para desplegar la sección.
33. Esta sección cuenta con 3 campos, uno para cada tipo de **Resolución** y a la derecha de cada campo se puede observar un botón deslizable. Desliza el botón correspondiente para indicar si la **Resolución** es requerida para activar el **Plan de Estudios** de una materia que se inserte dentro de una combinación dada de **Nivel de Estudio**.

{{<note text="A modo de ejemplo, si solo se activa la <b>Resolución Ministerial</b>, el <b>Plan de Estudios</b> de dicha carrera sólo se activará una vez que se emita la <b>Resolución Ministerial</b> y sin necesidad de que se emitan o expidan la <b>Resolución rectoral</b> y el <b>Expediente C.O.N.E.A.U.</b>.">}}

34. Haz clic en el botón **Guardar** y luego confirma los cambios realizados.
35. Verifica que los cambios se hayan guardado. Para ello, simplemente selecciona el **Nivel de Estudio**, y haz clic en la sección **Resoluciones requeridas** para verificar que las resoluciones que activaste se encuentren de hecho activas.

## Véase también

[Evaluaciones y Expresiones →]({{< relref "/evaluaciones-y-expresiones" >}} "Evaluaciones y Expresiones")

[Criterios de Regularidad →]({{< relref "/criterios-de-regularidad" >}} "Criterios de Regularidad")
