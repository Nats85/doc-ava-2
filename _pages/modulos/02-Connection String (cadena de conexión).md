---
title: Connection String (cadena de conexión)
chapter: "modulos"
---

Este módulo permite registrar las cadenas de conexión a la base de datos que posteriormente se utilizarán para el despliegue o actualización de una base de datos.

Para registrar una cadena de conexión siga los siguientes pasos:

1.	En la parte superior de la pantalla, seleccione el proveedor de base de datos. Las opciones son:

 •	SqlServer
 •	Oracle

2.	Asigne un nombre para identificar la conexión

3.	Registre los datos de conexión (nombre de la base de datos o TNS, nombre del servidor o dirección IP, y si se requiere usuario y contraseña).

4.	Haga clic en el botón Save (guardar).

![]({{ site.baseurl }}/assets/images/conexion 1.png)

Para probar la conexión y corroborar que sea correcta, haga clic en el botón Test, recibirá una alerta indicando si se pudo o no establecer la conexión.

Si luego de guardar desea editar o remover una cadena, haga clic derecho sobre el elemento en el listado y seleccione la opción que desee.

![]({{ site.baseurl }}/assets/images/conexion 2.png)

Notas:
 •	La base de datos debe existir, eso quiere decir que la base de datos debe crearse previamente en la instancia en la cual se va a desplegar.
 •	La aplicación se encarga solamente de crear y/o actualizar el esquema.

Si desea aplicar las cadenas a las aplicaciones instaladas, seleccione la cadena y haga clic en el botón Apply (aplicar) ubicado en la parte inferior derecha o a través del menú contextual. Se abrirá un cuadro de diálogo con el listado de aplicaciones y servicios disponibles en ese ordenador. Selecciónelos y haga clic en Apply (aplicar).

![]({{ site.baseurl }}/assets/images/conexion 3.png)

Si desea desplegar o actualizar las bases de datos, seleccione la cadena y haga clic en el botón Update (actualizar) ubicado en la parte inferior derecha o a través del menú contextual.

Continúe con los siguientes pasos:

1.	Seleccione la versión que desea desplegar o actualizar.
2.	Haga clic en el botón Update (actualizar).

![]({{ site.baseurl }}/assets/images/conexion 4.png)

El registro de información de la actualización muestra paso por paso las acciones que se están ejecutando y los errores que se puedan presentar.

![]({{ site.baseurl }}/assets/images/conexion 5.png)

Nota: Todos los errores se guardan en el archivo ADBT.LOG ubicado en la carpeta de Logs dentro de la carpeta de instalación de la aplicación.
