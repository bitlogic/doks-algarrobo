---
title: "Importar cátedras"
description: "Carga datos de cátedras de manera masiva."
lead: "Esta funcionalidad te permite cargar en el planificador múltiples cátedras y/o seminarios con todos sus detalles (modalidad, período, materia, cupo, docente, etc.) por medio de una plantilla con extensión .xls o .xlsx."
date: 2020-11-16T13:59:39+01:00
lastmod: 2020-11-16T13:59:39+01:00
draft: false
images: []
weight: 150
toc: true
---

{{<warning text="Para poder migrar masivamente la información de cátedras usando esta herramienta, primero debes tener disponible el archivo que se usa como plantilla de importación y que se entrega cuando el planificador está disponible en el entorno de producción. Una vez que tengas la planilla completa con los datos que se incluyen al final de este documento, la deberás guardar de manera local.">}}
</b>

1. Para comenzar, en el panel de navegación selecciona el icono de almacenamiento en la nube {{<inline-icon image="cloud upload.png" alt="upload icon">}} para acceder a la pantalla "Importación de cátedras".
1. Haz clic en el botón **Subir archivos** ubicado en el centro de la pantalla para cargar la plantilla con los datos de las cátedras que deseas cargar.
1. La ventana para seleccionar la plantilla desde el disco local se abrirá. Elige el archivo y haz clic en abrir. 
<br>

{{< tip text=`También puedes cargar el archivo arrastrándolo y soltándolo dentro de la ventana del importador.

` >}}
<br>

{{< note text=`Si la planilla ya existe se mostrará el siguiente mensajes: “El archivo que deseas subir ya existe. Intenta nuevamente modificando y guardando los cambios o subiendo otro archivo”. Esta funcionalidad también valida que se suba únicamente un archivo.

` >}}
</b>

4. El primer paso del proceso de importación de datos es el **Análisis de importación**. En esta instancia se verifica que la planilla no contenga errores u omisión de datos requeridos.
5. Si existe alguna inconsistencia en los datos, el proceso de importación se detiene en la etapa 2 **Detalle del análisis**. El sistema ofrece la opción de descargar un reporte con los errores dónde se incluyen detalles de las filas y columnas con su tipo de error. También se muestra un mensaje con la cantidad de errores en la parte superior de la pantalla. 
6. Si en esta etapa no se encuentran errores, puedes ver en la pantalla la cantidad de cátedras/seminarios analizados. Si lo deseas, puedes descargar este informe haciendo clic en el ícono de descarga.
7. Si la plantilla no contiene errores o inconsistencias en los datos, en el paso “Detalle del análisis” se habilita el botón **Cargar**.
8. Cuando los datos se comienzan a cargar, se inicia el proceso de importación de datos.
9. Al finalizar, se abrirá una ventana con un mensaje que confirma que la importación se realizó con éxito. Si se detectan errores, al igual que en el análisis, se indica cuántas cátedras se procesaron correctamente y cuantos errores hubo. También se genera un reporte detallado de errores disponible para descargar.
10. Haz clic en **Ver resumen** para controlar el total de cátedras/seminarios que se cargaron. 
11. En el paso 4 “Reporte de creación”, el sistema indica que la importación se completó. Si quieres, puedes presionar el botón **Volver a gestión** para regresar a la pantalla principal del planificador. Las cátedras/seminarios ya son parte del sistema y puedes cargar filtros en el buscador para verlos en la pantalla.

### Formato de la planilla de importación

El importador analiza el contenido de la planilla cargada. Por este motivo es importante tener en cuenta las siguientes especificaciones sobre el archivo .xls:

- El nombre de la hoja que contenga la información de las cátedras a importar debe ser “AULERO”, evitando incluir datos como el año o período.
- Los datos que se agreguen manualmente al archivo deben coincidir con los nombres que figuran en la base de datos. Por ejemplo, si en la base de datos figura como “CURSADO MODALIDAD PRESENCIAL 2-20”, se debe asegurar que el nombre en la plantilla se exactamente igual.
- La modalidad debe ser P, P. o PH. Actualmente viene como MP 1.
- La combinación de modalidad y sede debe ser correcta.
- El aula debe pertenecer al edificio seleccionado.
- La hora de fin de un módulo debe ser mayor a la hora de inicio.
- Las semanas de los encuentros Experimenta deben estar dentro del rango de fechas del subperíodo seleccionado.
- El plan de estudio (currículo) no puede estar vacío cuando la importación es para una modalidad a distancia.

#### Datos requeridos para la carga de datos:

| Nombre de la columna | Descripción | Ejemplos |
| -- | -- | -- |
| Sede | Lugar específico en donde se cursa una modalidad | SC
| Subperíodo | Subdivisión de un período académico | Período Académico 1-21 A - Marzo -Mayo 2021, Cursado cuatrimestral 1/22
| Modalidad | Modalidad de cursado | PH, P
| Edificio | Espacio físico en donde se dictarán las clases/encuentros | NVA. CBA, EXPERIMENTA 21, ARCOR
| Sala | Nombre del aula/sala | NC 409, LAB- 7.2, L-SOF 5
| Jornada | Turno de cursado | M, T, N
| Día | Día de la semana en el que se agenda la clase/encuentro | LUNES, MARTES, MIÉRCOLES
| Carrera | Código interno de la carrera | CPB, AAG, AYE, SIS
| Componente | Hace referencia al código utilizado para los tipos de cátedras y seminarios existentes | CAT, SEM, SEM-EXP
| Código asignatura | Código interno de la materia | ADO204, ECO204, INF243, DER324
| CAT/SEM | Código identificador de cada cátedra/seminario | AA, CM, 22, 45
| Profesor código | Código identificador del titular de la cátedra/seminario | 99999999
| Cupo | Máximo de estudiantes permitido | 42
| Currículo | Plan de estudio de la carrera | 7, 20, 6, 18
| Semanas Experimenta | Semanas del subperíodo en las que se producen los encuentros | 2,4,6,8,9
| Apertura | Orden de apertura de la cátedra/seminario a crear | 1, 2, 3, 4
| Num eventos | Para completar este campo se deben tener en cuenta las consideraciones* que se incluyen más abajo |
| Horario inicio | Hora de inicio de la clase/encuentro |
| Hora fin | Hora de finalización de la clase/encuentro |
---

_Información exclusiva de la Universidad Siglo 21_

*Consideraciones: recuerda que la duración de un módulo se define por la cantidad de eventos (horas cátedras) que lo componen. Cada evento tiene una duración de 40 minutos. Por ejemplo, un módulo compuesto por 2 eventos tendrá una duración de 80 minutos. Los módulos deben ser de 120 minutos como máximo. Por tal motivo, si fuese necesario que una cátedra tenga 4 eventos, se deberán crear 2 módulos con dos eventos cada uno. 
En la grilla se puede definir esta información de manera numérica usando los siguientes valores:
- 1, 2 y 3 eventos (<=3 eventos) corresponden a 1 Módulo (sin recreo).
- 4 y 5 eventos (>3 eventos <6) se deben dividir en 2 Módulos (con posibilidad de un recreo intermedio dependiendo de los horarios).
- 6 o más eventos (>=6 eventos) se deben dividir en 3 Módulos (con posibilidad de recreo intermedio dependiendo de los horarios en la base).
<br>

## Véase también

[Buscar cátedras →]({{< ref "buscar-catedras" >}} "Buscar cátedras")
<br/>
[Editar cátedras →]({{< ref "editar-catedras" >}} "Editar cátedras")
<br/>
[Abrir cátedras →]({{< ref "abrir-catedras" >}} "Abrir cátedras")
