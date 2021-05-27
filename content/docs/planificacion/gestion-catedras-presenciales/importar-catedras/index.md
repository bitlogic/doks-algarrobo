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

{{<warning text="Para poder migrar masivamente la información de cátedras usando esta herramienta, primero debes tener disponible el archivo que se usa como plantilla de importación y que se entrega cuando el planificador está disponible en el entorno de producción. Una vez que tengas la plantilla complete con los datos que se incluyen al final de este documento, se la deberá guardar de manera local.">}}
</b>

1. Para comenzar, en el panel de navegación selecciona el icono de almacenamiento en la nube {{<inline-icon image="cloud upload.png" alt="upload icon">}} para acceder a la pantalla "Importación de cátedras".
1. Haz clic en el botón **Subir archivos** ubicado en el centro de la pantalla para cargar la plantilla con los datos de las cátedras que deseas migrar.
1. La ventana para seleccionar la plantilla desde el disco local se abrirá. Elige el archivo y haz clic en abrir. 

{{< note text=`Si la planilla ya existe se mostrará el siguiente mensajes: “El archivo que deseas subir ya existe. Intenta nuevamente modificándolo o subiendo otro archivo”.

` >}}
</b>

4. El primer paso del proceso de importación de datos es el **Análisis de importación**. En esta instancia se verifica que la planilla no contenga errores u omisión de datos requeridos.
5. Si existe alguna inconsistencia en los datos, el proceso de importación se detiene en la etapa 2 **Detalle del análisis**. El sistema ofrece la opción de descargar un reporte con los errores dónde se incluyen detalles de las filas y columnas con su tipo de error. También se muestra un mensaje con la cantidad de errores en la parte superior de la pantalla. 
6. Si en esta etapa no se encuentran errores, puedes ver en la pantalla la cantidad de cátedras/seminarios analizados. Si deseas descargar este informe haciendo clic en el ícono de descarga.
7. Si la plantilla no contiene errores o inconsistencias en los datos, en el paso “Detalle del análisis” se habilita el botón **Cargar**.
8. Cuando los datos se comienzan a cargar, se inicia el proceso de importación de datos.
9. Al finalizar, se abrirá una ventana con un mensaje que confirma que la importación se realizó con éxito.
10. Haz clic en **Ver resumen** para controlar el total de cátedras/seminarios que se cargaron. 
11. En el paso 4 “Reporte de creación”, el sistema indica que la importación se completó. Si quieres, puedes presionar el botón **Volver a gestión** para regresar a la pantalla principal del planificador. Las cátedras/seminarios ya son parte del sistema y puedes cargar filtros en el buscador para verlos en la pantalla.

### Formato de la planilla de importación

El importador analiza el contenido de la planilla cargada por lo que deben seguirse las siguientes  especificaciones sobre el archivo .xls:

- El nombre de la hoja que contenga la información de las cátedras a importar debe ser “AULERO”, evitando incluir datos como el año o período.
- Los datos que se agreguen manualmente al archivo deben coincidir con los nombres que figuran en la base de datos. Por ejemplo, si en la base de datos figura como “CURSADO MODALIDAD PRESENCIAL 2-20”, se debe asegurar que el nombre en la plantilla se exactamente igual.
- La modalidad debe ser P, P. o PH. Actualmente viene como MP 1.

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

## Véase también

[Buscar cátedras →]({{< ref "buscar-catedras" >}} "Buscar cátedras")
<br/>
[Editar cátedras →]({{< ref "editar-catedras" >}} "Editar cátedras")
<br/>
[Abrir cátedras →]({{< ref "abrir-catedras" >}} "Abrir cátedras")
