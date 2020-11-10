---
title: Configuración previa en Aranda Service Desk
chapter: "configuracion"
---

En ASDK, se deben configurar dos nuevos grupos de trabajo: **Teams Manager** y **Teams Client**.

Así mismo se deben crear dos nuevos usuarios: **tmanager** y **tclient**.

Estos usuarios deben asociarse a los respectivos grupos de trabajo anteriormente creados y luego se les deben asignar los dos permisos correspondientes a cada grupo de trabajo así:

| __Grupo de trabajo y usuario__  | Permisos en la consola de administración __Aranda Service Desk BLOGIK__ | Permisos en la consola de especialistas __Aranda Service Desk FRONT END__ |
|-----------------------------|---------------------------------------------------------------------|-----------------------------------------------------------------------|
|   Teams Manager -> tmanager | ·         APPLICATION EXECUTE ·         TEAMS MANAGER               |                                                                       |
|   Teams Client -> tclient   |                                                                     | ·         APPLICATION EXECUTE ·         TEAMS CLIENT |

Posteriormente, en el servidor donde se encuentre instalada la aplicación de
Aranda Service Desk USDKv8 (consola de usuario) siga los siguientes pasos:

1.  Diríjase a la ruta de instalación (generalmente es
    C:\\inetpub\\wwwroot\\USDKV8) y una vez allí, ubique el archivo llamado
    Web.config

![]({{ site.baseurl }}/assets/images/5fd2adc56faedc753374c62731c03e0b.png)

2.  Abra el archivo con un editor de texto y ubique la siguiente línea:

    <`add name="X-Frame-Options" value="SAMEORIGIN" /`>

![]({{ site.baseurl }}/assets/images/14849444d140ce162040a517c35d7759.png)

3.  Una vez ubicada, reemplácela por la siguiente línea:

    <`add name="Content-Security-Policy" value="frame-ancestors 'self' teams.microsoft.com *.azurewebsites.net"/\`>

![]({{ site.baseurl }}/assets/images/fc8154177633b4eeecda11170d80061d.png)

4.  Valide que en los DNS configurados en la línea anterior se incluya el de su ambiente de Aranda, de lo contrario adiciónelo (\*.sudns.com).

5.  Guarde los cambios y reinicie el IIS.
