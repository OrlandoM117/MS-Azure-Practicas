# Practica9.
**En esta practica se vera como crear un Storage Account en Azure y como crear un container/blob storage, file storage, queue y tablas todo esto dentro del Storage Account que crearemos(Es necesario crear un storage account para poder crear estos recursos).**


--------------
## Recursos.
- Tener una suscripcion.
- Tener conexion a internet.
- Tener instalado un navegador (Brave,Google,Firefox, etc).

--------------
## Cosas a tener en cuenta.

--------------
## TUTORIAL.

**1.-Primero creamos un storage account**
![imagen1](imagenes/1.png)

**2-Ahora le damos la configuracion a nuestro storage account (Es importante saber que para crear un recurso lo minimo que tenemos que tener es -Una region, -Una suscripcion, -Un nombre, -Un grupo de recursos**
![imagen2](imagenes/2.png)

**3.-Aqui podemos ver los tipos de redundancia, escoge el mas adecuado para ti (En esta practica escogeremos la LRS)**
![imagen3](imagenes/3.png)

**4.-Ahora nos vamos a networking y permitimos que este el acceso publico a todas las redes**
![imagen4](imagenes/4.png)

**5.-Ahora le damos en revisar y en crear y creamos el storage account**
![imagen5](imagenes/5.png)

**6.-Ahora nos vamos al recurso**
![imagen6](imagenes/6.png)

### CONTAINERS/BLOB STORAGE
**7.-Ahora lo primero que haremos en crear un CONTAINER/BLOB STORAGE**
![imagen7](imagenes/7.png)

**8.-Le damos un nombre y que el acceso sea Container(anonymous read acces) y lo subimos**
![imagen8](imagenes/8.png)

**9.-Ahora probemos en cargar un archivo en Upload y seleccionando el archivo de nuestro windows con la interfaz de la izquierda**
![imagen9](imagenes/9.png)

**10.-Ahora podras ver que se subio el archivo y si lo seleccionamos nos mostrara lo siguiente podemos copiar la url y ver la imagen**
![imagen10](imagenes/10.png)

**11.-Aqui se puede ver el archivo que subimos (en este caso fue la imagen de un perrito)**
![imagen11](imagenes/11.png)

**12.-También podemos subir paginas estaticas a nuestro blob storage seleccionado web static en la interfaz de la izquierda y activando al opcion como se muestra a continuación**
![imagen12](imagenes/12.png)

**13.-Activando esta opcion nos mostrara los siguientes recuadros donde podremos poner el nombre de nuestra pagina**
![imagen13](imagenes/13.png)

**14.-Ahora nos regresamos a nuestro container y se nos creara un $web ahi podemos subir nuestros archivos de nuestra pagina web estatica como lo hicimos con la imagen del perrito, y si copiamos la url del archivo podemos visualizarlo o si queremos ver todo en conjunto copiamos la url de la interfaz static web podremos visualizarlo**
![imagen14](imagenes/14.png)

### FILE STORAGE

**15.-Para crear un file storage nos vamos a file shares en la misma cuenta de almacenamiento(storage account)**
![imagen15](imagenes/15.png)

**16.-Creamos uno nuevo, le ponemos un nombre el tipo de tier (en este caso le pondremos optimized-el basico) y lo creamos**
![imagen16](imagenes/16.png)

**17.-Ahora adentro del file storage podremos subir archivos dandole a upload y seleccionando el archivo desde la interfaz de la izquierda y subiendolo**
![imagen17](imagenes/17.png)

**18.-Aqui se podra ver tu archivo, en este ejemplo practico subí un archivo en .py llamado "holamundo"**
![imagen18](imagenes/18.png)

**19.-Si le damos click derecho encima de cualquier archivo lo podemos editar**
![imagen19](imagenes/19.png)

**20.-Como podras ver a continuación**
![imagen20](imagenes/20.png)

**21.-Ahora si queremos conectar este file storage a nuestra computadora e ir subiendo archivos mucho mas facil desde nuestro sistema operativo le damos en Connect y seleccionamos nuestro sistema operativo y copiamos el codigo que nos muestra a continuación**
![imagen21](imagenes/21.png)

**22.-Abrimos un PowerShell o Cmd y pegamos el codigo le damos enter despues de pegarlo**
![imagen22](imagenes/22.png)

**23.-Ahora como podras ver se nos muestra en nuestro equipo un disco extra que es el file storage y ahi podremos arrastrar los archivos para ir pegandolos mas facil o abrirlos desde ahi**
![imagen23](imagenes/23.png)

### QUEUE
**24.-Ahora para crear una queue nos dirigimos a la interfaz de la izquierda y seleccionamos queue (dentro desde nuestra storage account)**
![imagen24](imagenes/24.png)

**25.-Le damos un nombre a nuestra fila y la agregamos**
![imagen25](imagenes/25.png)

**26.-Desde nuestra queue podemos poner mensajes a cada uno, poner la expiracion o que nunca expire y le damos a ok para agregarlo a nuestra queue**
![imagen26](imagenes/26.png)

**27.-Como podras ver en overview se ven los mensajes de nuestra fila**
![imagen27](imagenes/27.png)


### TABLES
**28.-Ahora para crear tables nos dirigimos a la interfaz de la izquierda y seleccionamos Tables (recuerda que desde la misma cuenta de almacenamiento o si tu quieres crear otra cuenta de almacenamiento para crear una tabla)**
![imagen28](imagenes/28.png)

**29.-Aqui le damos un nombre a nuestra tabla y la agregamos le damos en OK**
![imagen29](imagenes/29.png)

**30.-Se muestran las tablas creadas pero para modificarlas tendremos que irnos a la interfaz de la izquierda y seleccionar storage browser(preview)**
![imagen30](imagenes/30.png)

**31.-Seleccionamos tablas y la tabla creada es usuarios la seleccionamos**
![imagen31](imagenes/31.png)

**32.-Aqui podremos ir añadiendo datos a nuestra tabla**
![imagen32](imagenes/32.png)

**33.-Como podras ver estos son los dos datos añadidos de mi tabla**
![imagen33](imagenes/33.png)

**FIN**

---------------------
