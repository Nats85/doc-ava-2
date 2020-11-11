---
title: Packages (paquetes)
chapter: "modulos"
---

El esquema de creación y actualización de la base de datos se realiza a través de la distribución de paquetes por versión. El módulo de paquetes permite descargar los paquetes de versiones de bases de datos a través de un servidor FTP o del sistema de archivo local (disco extraíble o memoria USB).

![]({{ site.baseurl }}/assets/images/paquetes 1.png)


Para descargar paquetes siga los siguientes pasos:

1. En la parte superior de la pantalla, seleccione el proveedor de base de datos. Las opciones son:
 •	SqlServer
 •	Oracle

2.	Seleccione el tipo de descarga. Las opciones son:
 •	Incremental: obtiene los paquetes que hacen falta (nuevas versiones) o los que no estén disponibles en la ubicación donde se almacenan.
 •	Total: sobrescribe los archivos existentes.

3.	Seleccione el origen de los paquetes. Las opciones son:
 •	Remote: la aplicación descarga los paquetes directamente de los servidores de Aranda. Si por políticas de red se requiere pasar por un proxy para tener salida a internet, haga clic en el botón Configure y registre la información del proxy.

![]({{ site.baseurl }}/assets/images/paquetes 2.png)

 •	FileSystem: el usuario descarga manualmente los paquetes según sean para Oracle o SQL desde la ruta http://download.arandasoft.com/ADBT/V9/ y los guarda localmente dentro de una carpeta que debe llamarse SQL u ORACLE según corresponda.
Una vez descargados, usando el botón Browse (explorar), indique la ruta en donde se hizo la descarga.

4.	Finalmente haga clic en el botón Download (descargar) para iniciar la descarga.
En el cuadro de descargas se puede observar el detalle del paquete con los siguientes datos: versión, proveedor, fecha de liberación, estado, dependencia, scripts iniciales y scripts incrementales. Si el estado es Not found (no encontrado), el paquete no está disponible y debe volver a descargarse.

![]({{ site.baseurl }}/assets/images/paquetes 3.png)

En la parte inferior se visualiza un registro de mensajes que indican las acciones que se están ejecutando o los errores que se pueden presentar durante la descarga.

![]({{ site.baseurl }}/assets/images/paquetes 4.png)
