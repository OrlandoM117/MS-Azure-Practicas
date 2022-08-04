# **Como conectar dos maquinas virtuales por medio de la nube de Azure**

**En esta practica veras como conectar dos maquinas virtuales por medio de la nube de azure**

![Logo de vm](imagenes/pcvm.png) ![Logo de Azure](imagenes/azure.png)
----------

## Requisitos:
- Tener una suscripcion en Azure
- Conexión a internet
- Una PC/LAPTOP

## Cosas a tener en cuenta
- Este servicio te cobra por hora prendida aunque no la estes utilizando (SI quieres que ya no te cobre tendras que apagarla)

----------
## TUTORIAL

**1.- Abrimos el [Portal de Azure](https://portal.azure.com/#home) y buscamos en el buscador Virtual Machine y la seleccionamos**
![Imagen 1](imagenes/1.png)

**2.- Ahora Creamos una maquina virtual en el apartado de +Create**
![imagen 2](imagenes/2.png)

**3.- Seleccionamos Azure Virtual Machine** 

![imagen 3](imagenes/3.png)


**4.- Ahora configuramos nuestra virtual machine en este ejemplo seleccionamos la región de Australia Central seleccionamos como iso Windows 10 Pro, version 21h2-Gen2, un tamaño de Standart_DS1_v2, ingresamos credenciales para crear el inicio de sesión, y importante seleccionar al final solamente RDP para abrirlo desde una aplicación de microsoft que en los siguientes puntos tocaremos. Recordemos que para crear un recurso se necesita minimo:**
- Suscripción
- Grupo de Recursos
- Región
- Un Nombre
  
![imagen4](imagenes/4.png) 


**5.- Ahora vamos al apartado de redes y debemos de replicar lo puesto en la screenshot**


![imagen5](imagenes/5.png)

**6.- Ahora le daremos en revisar y crear, una vez que Azure nos haya verificado que este todo correctamente, le daremos en Create**
![imagen6](imagenes/6.png)

**7.- Ahora creamos otra maquina virtual para conectarlas esta lleva exactamente igual a lo anterior (Se recomienda cambiar nombres para diferenciarlas) lo unico que cambia es en Networking (Redes) donde aqui pondremos la red virtual para que haya una conexión entre las dos maquinas virtuales. Como se ve a continuación**

![imagen 8](imagenes/8.png)


**8.- Le daremos en revisar y en crear de nuevo como anteriormente**

![imagen 9](imagenes/9.png)

**9.- Nos dirigiremos a todos los recursos**

![imagen 10](imagenes/11.png)

**10.- Seleccionamos nuestro grupo de recursos**

![imagen 11](imagenes/12.png)

**11.- Nos vamos preferentemente a nuestra primera maquina virtual creada**

![imagen 12](imagenes/13.png)

**12.- Nos vamos a la interfaz de la izquierda y seleccionamos el apartado que dice "Connect" seleccionamos en la parte de arriba RDP y descargamos el archivo**

![image 13](imagenes/14.png)

**13.- Ahora para poder abrir este archivo, descargamos desde la aplicacion de Microsoft Store , En Mac es igual, Igual que en Linux que lo puedes buscar. Descargamos la aplicacion "Escritorio Remoto de Microsoft"**

![imagen 14](imagenes/15.png)

**14.- Abrimos el RDP con la aplicación instalada anteriormente**

![imagen 15](imagenes/16.png)


**15..- Ahora nos pedira las credenciales para iniciar sesión se las damos y ahora nos mostrara la pantalla de inicio**
![imagen 16](imagenes/17.png)



**16.- Dejamos la configuracion por defecto**
![imagen 17](imagenes/18.png)

**17.- Ahora por mientras carga nuestro Windows nos vamos nuevamente a nuestro grupo de recursos y nos vamos a nuestro recurso de la red virtual**

![imagen 18](imagenes/19.png)

**18.- Nos vamos a la interfaz de la izquierda y seleccionamos Connect Devices y copiamos la dirección IP de la maquina virtual que nos queramos conectar en este caso es la segunda maquina virtual.**

![imagen 19](imagenes/20.png)

**19.- Ahora nos vamos nuevamente a nuestro Windows y damos click derecho en inicio y seleccionamos "Power Shell (Admin)"**

![imagen 20](imagenes/21.png)

**20.- Tecleamos el siguiente comando "mstsc (Direccion IP)**

![imagen 21](imagenes/22.png)

**21.- Ahora nos pedira nuestras credenciales de la segunda maquina virtual, se las daremos e ingresamos**

![imagen 22](imagenes/23.png)

**22.- Ahora estara iniciando nuestra segunda maquina virtual dentro de la primera maquina virtual**

![imagen 23](imagenes/24.png)

**23.- Nos pedira las configuraciones del Sistema, nuevamente se las dejamos como Default**

![imagen 24](imagenes/25.png)


**24.- Finalmente estaremos conectados entre las dos maquinas abriendo la primera maquina virtual y abriendo la otra maquina virtual**

![imagen 25](imagenes/26.png)

**25- Si no nos deja ingresar a la otra maquina virtual desde la primera por cualquier motivo puedes intentar tecleando el siguiente comando**

![imagen 26](imagenes/27.png)


