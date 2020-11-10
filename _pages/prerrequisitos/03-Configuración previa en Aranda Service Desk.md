---
title: Configuración previa en Aranda Service Desk
chapter: "prerrequisitos"
---

Se deben configurar dos nuevos grupos de trabajo: Teams Manager y Teams Client.
Así mismo se deben crear dos nuevos usuarios: tmanager y tclient.

Estos usuarios deben asociarse a los respectivos grupos de trabajo anteriormente creados y luego se les deben asignar los dos permisos correspondientes a cada grupo de trabajo así:

![]({{ site.baseurl }}/assets/images/3.png)

Posteriormente, en el servidor donde se encuentre instalada la aplicación de Aranda Service Desk USDKv8 (consola de usuario):

  a) Diríjase a la ruta de instalación `(generalmente es C:\inetpub\wwwroot\USDKV8)` y una vez allí, ubique el archivo llamado Web.config

![]({{ site.baseurl }}/assets/images/4.png)

b) Abra el archivo con un editor de texto y ubique la siguiente línea: `<add name="X-Frame-Options" value="SAMEORIGIN" />.`


![]({{ site.baseurl }}/assets/images/5.png)

c) Una vez ubicada, reemplácela por la siguiente línea:`<add name="Content-Security-Policy" value="frame-ancestors 'self' teams.microsoft.com*.azurewebsites.net"/>`

![]({{ site.baseurl }}/assets/images/6.png)

d) Guarde los cambios y reinicie el IIS.
