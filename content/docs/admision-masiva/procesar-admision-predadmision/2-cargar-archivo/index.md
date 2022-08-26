---
title: "Paso 2 - Cargar archivo"
lead: "Carga un archivo del tipo .csv que contenga los datos de los estudiantes a admitir o a pre admitir."
date: 2022-07-24T15:56:41-0300
lastmod: 2020-11-16T13:59:39+01:00
draft: false
images: []
weight: 150
toc: true
---

1. Descarga un _template_ o plantilla haciendo clic en el vínculo que se muestra en la segunda nota debajo del botón **Cargar archivo**.
2. Una vez descargado el archivo, procede del siguiente modo para abrirlo:
    - Primero de todo, abre Excel y crea un nuevo Libro.
    - A continuación, ve a la pestaña **DATOS**, y luego desde la sección "Obtener datos externos", selecciona "Desde un archivo de texto". Se desplegará la ventana de explorador llamada "Importar archivo de texto" para buscar y seleccionar el archivo CSV que queremos abrir - el template que descargaste.
    - En este explorador, haz clic en la lista desplegable que se encuentra junto al campo **Nombre de archivo** y selecciona "Todos los archivos" (\*\.\*\). Esta opción te permite visualizar la plantilla (template.csv) recién descargada (se descarga en la carpeta "Descargas") para así seleccionarla.
    - Una vez seleccionada la plantilla template.csv, haz clic en el botón **Importar**. Se abrirá la ventana "Asistente para importar texto - paso 1 de 3".
    - Deja la selección que aparece marcada por defecto **Delimitados** y haz clic en **Siguiente**.
    - Selecciona la **Coma** como delimitador. Haz clic en **Siguiente**.
    - Deja la pantalla tal cual está, y haz clic en **Finalizar**.
    - En la ventana que se despliega, haz clic en **OK** para que la plantilla se vea en la hoja de trabajo actual. Así obtendrás la Plantilla con el formato que necesitas para armar la lista de estudiantes a ser admitidos.

3. Una vez que tengas la Plantilla, completa el archivo con los siguientes datos de los estudiantes a admitir o a pre admitir en el formato que se indica a continuación:
   - **Nombre:** y **Apellido:** Sólo letras
   - **e-mail:** Debe contener el  signo @ (arroba), el nombre de usuario delante y el dominio detrás
    - **Fecha de nacimiento:** DD/MM/AAAA
    - **Tipo de documento:** S/D, DNI, LE, LC, PASAPORTE, y CEDULA (en donde S/D significa “sin datos” y Cédula se escribe sin tilde)
    - **Número de documento:** Sólo números
    - **Género:** F o M
    - **País:**, **Provincia:**, y **Localidad:** Sólo letras
    - **Estado civil:** SOLTERO, CASADO, DIVORCIADO, S/D, SEPARADO, VIUDO (en donde S/D significa “sin datos”)

{{<warning text="Debes respetar el formato arriba detallado para que el resultado de la carga del archivo no de errores y la admisión pueda realizarse.">}}
</b>

4. Por último, guarda el archivo mediante la opción “Guardar como” en una carpeta en tu ordenador y **asegúrate de guardarlo como archivo CSV** (Comma delimited) (*.csv).

{{<note text="Guárdalo con un nombre que puedas reconocer fácilmente, por ejemplo, con el nombre que utilizaste para nombrar la Admisión: Admisiones_GrupoABC.csv.">}}
</b>

5. Una vez que el archivo esté listo, haz clic en el botón **Cargar archivo** para localizarlo en tu PC y seleccionarlo, o selecciona el archivo y arrástralo hacia la nueva ventana desplegada. El sistema informará que el archivo fue seleccionado, y si por algún motivo debes cambiarlo por otro, podrás eliminarlo al hacer clic en la **marca de cruz** {{<inline-icon image="round_close_black_24dp.png" alt="close icon">}} que se encuentra a la derecha del archivo.
6. Haz clic en el botón **Siguiente**. En la sección "Resumen de la importación", la app te advertirá que está procesando la información ingresada y luego te indicará si la importación se realizó con éxito al desplegar:
   - un botón con la leyenda Error y el número de errores encontrados
   - un botón donde se lee Ok y el número de estudiantes admitidos con éxito
   - un botón donde se lee **Total** que indica la cantidad total de estudiantes que se intentaron admitir 

{{<note text="Una vez importado el archivo con la información de los estudiantes, en la ventana Resultado de la importación también podrás ver la sección Datos de la oferta académica la cual contiene los datos seleccionados en el Paso 1.">}}
</b>


## Véase también

[Paso 1 - Datos de la oferta académica →]({{< relref "/1-datos-oferta-academica" >}} "Paso 1 - Datos de la oferta académica")
</b>

[Paso 3 - Resultado de la importación →]({{< relref "/3-resultado-importacion.md" >}} "Paso 3 - Resultado de la importación")