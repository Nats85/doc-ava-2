---
title: Configuración de Aranda Virtual Agent en Teams
chapter: "configuracion"
---

Para configurar el servicio de Aranda Virtual Agent en Teams siga los siguientes pasos:

**a).** Haga clic en la pestaña **Configuración**.

![]({{ site.baseurl }}/assets/images/12.png)

**b).** Ingrese los siguientes datos en los campos solicitados y haga clic en **Ingresar:**

- **USDK BackEnd Url:** https://servidoraranda/ASDKAPI/

- **Usuario:** tmanager

- **Contraseña:** ABC123

- **Email Corporativo:** (usuario@arandasoft.com)

- **Versión:** V8

Aparecerá la siguiente ventana emergente:

![]({{ site.baseurl }}/assets/images/13.png)

**c).** Ingrese los siguientes datos en los campos solicitados y haga clic en **Crear:**

- **USDK Front End:** URL de la consola USDKV8.

- **USDK Back End Url:** URL del API de ASDKV8.

- **Usuario:** usuario TEAMS CLIENT (tclient)

- **Contraseña:** contraseña Usuario TEAMS CLIENT.

- **Email Corporativo:** (usuario@arandasoft.com)

- **Versión:** V8

- **Activa:** marcar la casilla


Aparecerá la siguiente ventana con la configuración realizada:

![]({{ site.baseurl }}/assets/images/14.png)


**d).** Diríjase a App Studio (puede encontrar App Studio con la ayuda del buscador de Aplicaciones en
Teams), y en la pestaña a **Manifest editor** seleccione la aplicación Aranda Virtual Agent.

![]({{ site.baseurl }}/assets/images/15.png)


**e).** Diríjase a la opción **Test and distribute** y luego haga clic en **Install**.

![]({{ site.baseurl }}/assets/images/16.png)

**f).** Haga clic en la flecha ubicada al lado derecho de **Agregar** y seleccione **Agregar a un equipo** o
**Agregar a un chat**, según requiera. El chat o equipo debe haberse creado y configurado previamente
en Teams de acuerdo a las necesidades o utilización que se le vaya a dar al bot.

![]({{ site.baseurl }}/assets/images/17.png)

**g).** Busque el chat o equipo y haga clic en **Configurar un bot.**

![]({{ site.baseurl }}/assets/images/18.png)
![]({{ site.baseurl }}/assets/images/19.png)

Al finalizar la configuración, automáticamente llegará al chat un mensaje de saludo del bot de Aranda Virtual
Agent.
