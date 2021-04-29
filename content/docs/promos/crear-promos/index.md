---
title: "Crear promociones comerciales"
description: "Con esta herramienta puedes configurar promociones comerciales que se aplicarán a los tickets."
lead: "Con esta herramienta puedes configurar promociones comerciales que se aplicarán a los tickets. Los descuentos aplicados a cada ticket se podrán ver desde la herramienta de ePagos. Las promociones comerciales pueden configurarse para asignar un monto fijo o un porcentaje que luego se aplicará al total del ticket que el estudiante debe abonar."
date: 2020-11-16T13:59:39+01:00
lastmod: 2020-11-16T13:59:39+01:00
draft: false
images: []
menu:
  docs:
    parent: "Promociones Comerciales"
weight: 050
toc: true
---

1. Ingresa a la herramienta de "Gestión de ingresos".
2. En el panel de navegación, selecciona el icono ![](../Documents/Markdown%20Monster%20Weblog%20Posts/prom.png) para que puedas acceder a la pantalla "Promociones comerciales". 
3. Haz clic en el botón ![](../Documents/Markdown%20Monster%20Weblog%20Posts/nueva.png) para comenzar.
4. En la pantalla “Nueva promoción”, comienza a completar los campos con los datos de la promoción que quieres crear. Selecciona en primer lugar si el descuento va a corresponder a un monto fijo o un porcentaje.

5. Luego, completa el nombre y descripción, selecciona el tipo de estudiante, el período y la validez de la promoción.

![](../Documents/Markdown%20Monster%20Weblog%20Posts/note2.png)

{{<note text="La definición del tipo de estudiante llamado \"Nuevo inscripto\" hace referencia a un estudiante que acaba de ingresar a la carrera. Mientras que el término \"Re-inscripto\" abarca a aquellos estudiantes que han cursado esa carrera anteriormente.">}}


6. Activa la promoción deslizando el botón de "Estado" hacia la derecha. Para desactivarlo, deslízalo hacia la izquierda. Si se encuentra marcado en verde significa que la promoción está activa.

7. En la pestaña "Tickets" puedes optar por el tipo de arancel y tickets a los que afectará esta promoción.

8. Dirígete a la pestaña "Criterios" (ubicada a la derecha de “Tickets”). Aquí podrás configurar las reglas que se considerarán para hacer efectivo el descuento


{{<note text="Los criterios que definas aquí indican a quiénes aplica y cuál es el monto o porcentaje de la promoción. Por eso es importante aclarar que cada regla \"incluye\" la población destino y al mismo tiempo \"excluye\" al resto de las opciones que no se han mencionado en esa definición. Entonces, si no se definen criterios, la promoción aplica a \"todos\". En cambio, si se incluye al menos una combinación para un segmento de población, habrá que configurar entonces qué sucede con el resto de las opciones que quedan automáticamente excluidas. Para más detalles, ve a la siguiente nota.">}}


9. Haz clic en el icono de "Entradas" ![](../Documents/Markdown%20Monster%20Weblog%20Posts/entrada.png) para elegir la población para quiénes aplican estas reglas. Puedes optar entre: Región, Modalidad, SubModalidad, Clase estudio, Carrera, Sede/CAU, Turno, Marca y Paquete. Todas estas opciones tienen listas desplegables. 
10. En las columnas de salida, dentro del campo "Valor" puedes definir el monto de la promoción o el valor del porcentaje dependiendo del tipo de promoción seleccionado.

11. Si deseas configurar esta promoción para que su aplicación abarque diferentes opciones de población, tendrás que seleccionar el botón ![](../Documents/Markdown%20Monster%20Weblog%20Posts/agregar%20prom%20comercial.png) y definir estos valores para todos los escenarios.

![](file:///C:\Users\vbrue\Documents\Markdown%20Monster%20Weblog%20Posts\note2.png)

{{<note text=`Las reglas se aplican con un orden de prioridad de arriba hacia abajo. Puedes agregar tantas reglas como desees. Las siguientes acciones están disponibles en esta grilla:
<br>
- Clonar: si una regla ya está definida, al hacer clic en este icono puedes copiar debajo exactamente la misma información.
<br>
- Ordenar: cuando tengas varias reglas y quieras asignarles un nuevo orden en la grilla, puedes hacer clic en este ícono en el renglón de la regla que deseas mover y arrastrarla hacia su nuevo lugar. La herramienta te informa acerca de esta posibilidad con un mensaje en la parte inferior de la grilla.
<br>
- Eliminar: usa este botón para eliminar una regla. 
<br>
Por último, si has incluido varios criterios, será necesario que en la última fila definas cómo se aplicará la promoción a la parte de la población excluida. Si colocas un \"0\" en el campo valor, esto significa que no se desea incluir ningún otro tipo de población a la promoción y si ingresas otro valor (por ejemplo, \"5\") este descuento será aplicado al resto de la población que se excluyó en los criterios anteriores.`>}}

12.  Una vez definidos los datos generales de la promoción, los tickets asociados y las reglas o criterios de aplicación haz clic en el botón **Guardar.**

##### Véase también

[Buscar promociones comerciales]({{< relref "buscar-promos" >}})

[Editar promociones comerciales]({{< relref "editar-promos" >}})
