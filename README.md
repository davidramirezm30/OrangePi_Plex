# OrangePi_Plex
En este repositorio sive como guía para aprender instalar Plex Media Server en una Orange Pi con sistema operativo DietPi y cómo configurarla para sacarle el mayor partido.
He utilizado una Orange Pi PC, una tarjeta SD de 16 GB, un cable ethernet para conectar la Orange Pi al router y un disco duro externo de 1TB donde meter las películas, series, música...


## Instalación del Sistema Operativo en la OPI
Lo primero de todo es ir a la [web oficial de DietPi](http://dietpi.com) y descargarse el software que necesita tu Orange Pi y extraerlo.

![alt text](https://github.com/davidramirezdrm/OrangePi_Plex/blob/master/images/DietPi%20web.png)

Después hay que formatear la tarjeta SD y utilizando el programa [Win32 Disk Imager](https://sourceforge.net/projects/win32diskimager/) elegir la imagen DietPi.img y la tarjeta de memoria que donde se va a meter el SO y darle a Write.

![alt text](https://github.com/davidramirezdrm/OrangePi_Plex/blob/master/images/Win32%20Disk%20Imager.png)

Una vez hecho esto hay que meter la tarjeta en la Orange Pi, enchufarla a la corriente y poner el cable ethernet conectando el router y la Orange Pi. 

## Conseguir la IP de la Orange Pi
Una vez conectado hay que conseguir la dirección IP de la Orange Pi para conectarse por ssh. Una forma fácil de conseguirla es accediendo al router poniendo en el navegador 192.168.1.1 o 192.168.0.1 y poner el [usuario y contraseña](https://www.testdevelocidad.es/2016/12/12/usuario-contrasena-routers/)  que venga por defecto. Una vez dentro buscar una pestaña que ponga DHCP y ahí vendrán listadas todas las IPs que haya conectadas.

## Instalar todo lo necesario
Para acceder a la Orange Pi yo utilizo el bash de windows. La IP de mi Orange Pi es 192.168.1.100 así que mediante el comando _ssh root@192.168.1.100_. El usuario es root y la contraseña dietpi. 

Una vez dentro lo primero que hay que hacer es poner _dietpi-launcher_. Desde este menú se puede acceder a todos los menús principales que tiene DietPi y que facilita mucho la instalación.

Después de esto elegir Dietpi-Software y dentro de este menú entrar de nuevo en Software Optimized. Dentro de este menú seleccionar con la tecla espacio lo que queréis instalar, en mi caso yo he instalado:
+ 42  Plex Media Server: web interface media streaming server
+ 146 PlexPy: monitoring and tracking tool for Plex
+ 44  Transmission: bittorrent server with a web interface (c)
+ 67  NoIp: url website address for your device
 

