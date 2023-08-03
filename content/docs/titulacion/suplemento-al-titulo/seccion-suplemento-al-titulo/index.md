---
title: "Suplemento al título"
lead: "La sección Suplemento al Título se añade al Analítico para evidenciar las actividades co-curriculares completadas por un estudiantes al momento de la Titulación."
date: 2022-09-23T11:17:02-0300
lastmod: 2020-11-16T13:59:39+01:00
draft: false
images: []
weight: 150
toc: true
---


## Gestión de actividades co-curriculares

Las actividades co-curriculares se modelan como carreras, y por eso tienen:

- Nombre, Plan de Estudios, Director/a, etc.
- Una estructura curricular compuesta por las materias que deben aprobarse para completar la actividad

    {{<note text="Los números de las resoluciones son valores estáticos y <b>no</b> están relacionados con la actividad aprobada sino con las resoluciones que definió el ministerio para suplementos al título y el Consejo para créditos y suplementos.">}}

El **_Suplemento al Título_** se agrega al Analítico Final de forma automática mediante un proceso interno. Al iniciar el proceso de Titulación, se buscan todas las actividades co-curriculares que el estudiante haya completado y se agrega para cada una de ellas el siguiente texto:

_Certifico que <span style="color:blue">**\<Nombre de estudiante>**</span>, complementariamente a las materias de su plan de estudios, ha acreditado con éxito la actividad extracurricular <span style="color:blue">**\<Nombre de la actividad>**</span>, conforme al régimen aprobado por Resolución del Consejo Superior Nro <span style="color:blue">**\<Número de Resolución>**</span>, en armonía con lo dispuesto por Resolución Ministerial <span style="color:blue">**\<Número de Resolución Ministerial>**</span>._

## Créditos académicos

Las actividades co-curriculares que según la resolución otorgan créditos académicos se materializan en la aprobación de materias electivas en la carrera de grado que cursa el estudiante.

Por ejemplo, una resolución podría especificar que al completar la actividad co-curricular **Ayudante de cátedra** se otorgará una materia electiva. Sin embargo, para que esto suceda, los encargados de actualizar y mantener el sistema de equivalencias, deberán haber cargado las reglas correpondientes.

**Ejemplo:**

- Ayudantía IV equivale a Electiva I (con aprobación manual) resolución 4056/2020
- Ayudantía IV equivale a Electiva II (con aprobación manual) resolución 4056/2020

La **Regla de equivalencia** luego se disparará cuando el estudiante apruebe la última materia de la actividad co-curricular.

{{<note text="Se cargan ambas reglas puesto que algunos estudiantes pueden tener Electiva I aprobada al momento de completar la actividad y es el operador quien debe elegir cuál otorgar.">}}

## Véase también

[Descargar documentos →]({{< relref "/descarga-de-documentos" >}} "Descargar documentos")

[Agregar texto adicional al Analítico →]({{< relref "/agregar-texto-adicional-analitico" >}} "Agregar texto adicional al Analítico")

