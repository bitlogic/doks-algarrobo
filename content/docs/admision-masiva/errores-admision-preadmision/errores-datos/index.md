---
title: "Errores a nivel datos"
lead: "Conoce el tipo de errores a nivel de datos del registro que impiden el procesamiento de una admisión o pre admisión."
date: 2022-07-24T13:38:22-0300
lastmod: 2020-11-16T13:59:39+01:00
draft: false
images: []
weight: 150
toc: true
---

1. Cuando existe un error en los datos cargados, la app **Admisión masiva** te lo advertirá mediante el indicador de Error (círculo con un número) del "Resultado de la importación". Un error podría ser que en un registro (la admisión de 1 estudiante):
   - el tipo de dato no se corresponda con el campo: _por ejemplo, se ingresaron números en el campo_ **Nombre**
   - el formato del dato no sea como debería ser: _por ejemplo, el_ **email** _no tiene_ @
   - no se ingresó nada: _hay campos que se dejaron en blanco_
   - el estudiante ya fue admitido: _el estudiante fue admitido o pre admitido a la carrera indicada en el_ **Paso 1**
2. Para ver en detalle cuáles registros dieron error y cuál fue el error, descarga el archivo “Resultado de la importación”. A continuación, se describen 2 ejemplos de errores posibles:
    - Si ingresaste por equivocación en el campo **Nombre** un número o una serie de letras y números, por ejemplo, **Marcel0** (número cero en vez de la letra "o"), en la columna **Resultado** se observa la palabra ERROR, y en la columna **Mensaje** se desplegará _Nombre inválido_.

    - Si cargaste los datos de estudiantes que ya han sido admitidos a una carrera determinada, en la columna **Resultado** se observa la palabra ERROR, y en la columna Mensaje se lee _"El estudiante ya está registrado en la carrera elegida. Legajo del estudiante: VAGB126014_.”

{{<note text="Podrás cargar un estudiante ya admitido a una carrera porque este proceso lo que crea, es un Legajo, y el estudiante podría estar inscribiéndose a una segunda carrera, para la que tendrá un segundo Legajo. Por lo tanto, para admitir a un estudiante a una carrera diferente de la que ya ha sido admitido, deberás crear una admisión nueva.">}}
</b>

{{<warning text="Los registros que dan error NO logran terminar el proceso de admisión o pre admisión y por lo tanto NO se crea ni el Usuario ni el Legajo del estudiante.">}}
</b>

## Véase también
[Errores a nivel archivo →]({{< relref "/errores-archivo" >}} "Errores a nivel archivo")