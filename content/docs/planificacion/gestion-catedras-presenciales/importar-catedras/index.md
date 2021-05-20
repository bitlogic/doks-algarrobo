---
title: "Importar cátedras"
lead: "Esta funcionalidad te permite cargar en el planificador múltiples cátedras y/o seminarios con todos sus detalles (modalidad, período, materia, cupo, docente, etc.) por medio de una plantilla con extensión .xls o .xlsx."
date: 2020-11-16T13:59:39+01:00
lastmod: 2020-11-16T13:59:39+01:00
draft: false
images: []
weight: 150
toc: true
---

1. En el panel de navegación selecciona el icono correspondiente para acceder a la pantalla "Importación de cátedras".
1. Haz clic en el botón para subir archivos {{<inline-icon image="cloud upload.png" alt="upload icon">}}.
1. La ventana para seleccionar la plantilla desde el disco local se abrirá. se inicia el proceso de análisis e importación de los datos.
1. Si la planilla ya existe se muestra el siguiente error: “El archivo que desea subir ya existe. Intente nuevamente modificándolo o subiendo otro archivo”.
1. El primer paso es el análisis de importación. En esta instancia se verifica que la planilla no se haya subido antes y que no contenga errores u omisión de datos requeridos.
1. Si existe alguna inconsistencia en los datos, el proceso de importación se detiene en la etapa “Detalle del análisis”. El sistema ofrece la opción de descargar un reporte con los errores (1). Éste incluye detalles de las filas y columnas con su tipo de error. También se muestra un mensaje con la cantidad de errores (2) en la parte superior de la pantalla.
1. En el detalle del análisis se incluyen la cantidad de cátedras/seminarios analizados. Si desea, puede descargar  este informe haciendo clic en el ícono de descarga (3).
1. Si la planilla no contiene errores o inconsistencias en los datos, en el paso “Detalle del análisis” se habilita el botón “Cargar”.
1. Cuando los datos se comienzan a cargar se inicia el proceso de importación de datos.
1. Al finalizar se muestra el siguiente mensaje que indica que la importación se realizó con éxito.
1. Si hace clic en “Ver resumen” podrá ver el total de cátedras/seminarios cargados. En el paso 4 “Reporte de creación” se indica que la importación está completa.
1. Haga clic en “Volver a gestión” para volver a la pantalla principal del planificador. Las cátedras/seminarios de la planilla son parte del sistema.

### Formato de la planilla de importación

El importador analiza el contenido de la planilla cargada por lo que deben seguirse las siguientes  especificaciones sobre el archivo .xls:

- El nombre de la hoja que contenga la información de las cátedras a importar debe ser “AULERO”, evitando incluir datos como el año o período.
- Los datos agregados manualmente al archivo deben coincidir con los nombres como figuran en la base de datos. Ejemplo: si en la DB figura como “CURSADO MODALIDAD PRESENCIAL 2-20”, se debe asegurar que en la planilla no se carguen con diferencias (“CURSADO MODALIDAD PRESENCIAL 2/20”).
- La modalidad debe ser P, P. o PH. Actualmente viene como MP 1

#### Datos requeridos para la carga de datos:

| Nombre de la columna | Descripción | Ejemplos |
| -- | -- | -- |
| fsdf | Lugar específico en donde se cursa una modalidad | SC
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
| Cupo | Máximo de alumnos permitido | 42
| Currículo | Plan de estudio de la carrera | 7, 20, 6, 18
| Semanas Experimenta | Semanas del subperíodo en las que se producen los encuentros | 2,4,6,8,9
| Apertura | Orden de apertura de la cátedra/seminario a crear | 1, 2, 3, 4
| Num eventos | Cantidad de eventos que conforman una cátedra |
| Horario inicio | Hora de inicio de la clase/encuentro |
| Hora fin | Hora de finalización de la clase/encuentro |
---

_Información exclusiva de la Universidad Siglo 21_
