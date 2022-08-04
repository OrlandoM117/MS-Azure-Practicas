# Conectar dos Maquinas virtuales por medio de dos redes virtuales
**En esta practica se verá como conectar dos maquinas virtualos por networkvirtuals con imagen ubuntu**

![VM](imagenes/virtualmachine.png)![VN](imagenes/virtualnetwork.png)![Azure](imagenes/azure.png)
---------------

## Requisitos
- Tener una suscripcion Azure
- Tener conexion a internet
- Tener un navegador instalado
- 
---------------

## Cosas a tener en cuenta
- Las redes virtuales no te cobran pero las maquinas virtuales si
- Las maquinas virtuales te cobran por hora aunque no las estes utilizando (Es importante desactivarlas si no las vas a utilizar ya que te seguiran cobrando siempre y cuando esten encendidas)

---------------

## TUTORIAL
**1.-Primero que hay que hacer es crear las redes virtuales, creamos una**

![imagen1](imagenes/1.png)

**2.-Ahora en la configuracion de la red virtual recordemos que para crear un recurso lo minimo que tiene que tener es -Una suscricpion, -Un grupo de recursos, -Un nombre, -Una región. Una vez sabiendo esto podemos ir al tercer paso**

![imagen2](imagenes/2.png)

**3.-Nos Dirigimos a IP Addrresses y en subnet name podemos dejar la que esta por default o podemos cambiarle el nombre eliminandola y creando una nueva con la misma ip addres para que la subnet se conecte con la net virutal**

![imagen3](imagenes/3.png)

**4.-Ahora le daremos en revisar y crear**

![imagen4](imagenes/4.png)

**5.-Creamos otra red virtual recordemos cuales son las minimas especificaciones para crear una**

![imagen5](imagenes/5.png)

**6.-Nuevamente nos vamos ahora a nuestra net virtual 2 y seleccionamos IP Addresses y le damos una subnet nueva o dejamos por default la que tenia (los mismos pasos que la virtual network 1)**

![imagen6](imagenes/6.png)

**7.-Ahora le damos en revisar y en crear**

![imagen7](imagenes/7.png)

**8.-Ahora creamos la primera maquina virtual (recordemos las especificaciones minimas para crear un recurso) sabiendo esto ponemos la imagen iso como Ubuntu (En este caso de la practica se escogera ubuntu pero es lo mismo con windows) ponemos el tamaño de la maquina virtual que tenga una contraseña introducimos credenciales nuevas(es importante que te acuerdes de las credenciales ya que las utilizaremos mas adelante) activamos todos los puertos seleccionados y pasamos al siguiente paso**

![imagen8](imagenes/8.png)

**9.- En nuestra maquina virtual nos dirigimos a networking y es importante que la virtual network este en la numero uno y la subnet haya sido la primera (osea la net y la subnet de la primera red virtual que creamos)**

![imagen9](imagenes/9.png)

**10.-Ahora le damos en revisar y en crear**

![imagen10](imagenes/10.png)


**11.-Creamos otra maquina virtual (seguimos los mismos pasos que en la otra)**
![imagen11](imagenes/11.png)


**12.-Y ahora en networking escogemos virtualnetworking la segnuda red virtual creada y en subnet la subnet de la segunda red virtual**

![imagen12](imagenes/12.png)

**13.-Ahora le damos en revisar y en crear**

![imagen13](imagenes/13.png)

**14.-Nos dirigos preferentemente a la primera maquina virtual creada nos vamos a la interfaz de la izquierda seleccionamos "Connect" y en SSH en la opcion 4 copiamos los datos que aparecen adentro del circulo rojo**

![imagen15](imagenes/15.png)

**15.-Ahora nos vamos al portal de azure y abrimos un Azure Cloud Shell y le damos en bash (Puede ser tambien powershell) Si nos pide crear una cuenta de almacenamiento creamos una**

![imagen16](imagenes/16.png)

**16.-Ahora en esta ventana de bash ponemos ssh "pegamos aqui lo que habiamos copiado"**

![imagen17](imagenes/17.png)

**17.-Escribimos "yes" que si nos queremos conectar**

![imagen18](imagenes/18.png)

**18.-Ahora nos pedira nuestra contraseña escribimos la contraseña de la maquina virtual (En este caso estamos en la uno)**

![imagen19](imagenes/19.png)

**19.-Y una vez dentro te podras dar cuenta que ya no estamos en azure ahora estamos en nuestra maquina virtual de ubuntu**

![imagen20](imagenes/20.png)

**20.-Para comprobar para ver si estamos dentro podemos escribir "sudo apt-get moo" que se nos mostrara una vaquita**

![imagen21](imagenes/21.png)

**21.-Ahora para poder conectar las maquinas virtuales nos vamos a la red virtual 2 y en la interfaz de la izquierda seleccionamos connect devices**

![imagen22](imagenes/22.png)

**22.-Aqui copiamos la IP Address de la red virtual 2**

![imagen23](imagenes/23.png)

**23.-Nos regresamos a nuestro Azure cloud shell (importante no haber cerrado esta ventana si no tendremos que hacer los comandos de cloud shell anteriormente hechos) aqui ponemos ping "IPADDRESS" y ahora como podras ver no se conectan para resolver este problema haremos lo siguientes pasos**

![imagen24](imagenes/24.png)

**24.-Nos vamos a la red virtual 1 y nos vamos a la interfaz de la izquierda y selecccionamos Peerings y agregamos una nueva**

![imagen25](imagenes/25.png)

**25.-Una vez aqui adentro en nuestra red virtual uno le decimos un nombre en Peering link name(por tradicion se pone las redes virtuales que se van a conectar) y en remote virtual network (las escribimos al revez por tradicion) seleccionamos una suscripcion y en virtual network ponemos la red virtual a la que nos vamos a conectar en este caso la num2 y añadimos**

![imagen26](imagenes/26.png)

**26.-Nos vamos a la interfaz de la izquierda y nos vamos nuevamente a Peerings y hasta que nos salga en "Connect" nuestra nueva conexion significa que que podremos hacer nuestro ping**

![imagen27](imagenes/27.png)

**27.-Hacemos el mismo comando ping "IPAddress" y ahora como podras ver ya se conectaron "Felicidades"!!!**

![imagen28](imagenes/28.png)