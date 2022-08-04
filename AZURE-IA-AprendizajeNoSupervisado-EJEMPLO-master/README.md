# **IA APRENDIZAJE NO SUPERVISADO**

**En esta practica verás como una Inteligencia Artifical recrea un video de acuerdo a la palabra que tu le indiques.**


![Logo IA NOS](https://github.com/OrlandoM117/IA-AprendizajeNoSupervisado-EJEMPLO/blob/master/imagenes/aprendizajensia.png) ![Video Dog](https://github.com/OrlandoM117/IA-AprendizajeNoSupervisado-EJEMPLO/blob/master/imagenes/7.png)
------------------------------------------
## **Requisitos**:

- Tener Una PC Con sistema operativo Windows/Linux/Mac.
- Tener Conexión a Internet  
- Tener un navegador instalado pueden ser Google, Brave, Microsoft Edge, El de tu preferencia.

## **Bonus**:

- Si tienes una tarjeta gráfica dedicada de la marca NVIDIA puedes usar esta para obtener mejores resultados
- Si tienes una tarjeta gráfica dedicada de cualquier otra marca la puedes utilizar para obtener mejores resultados (No obtendrás los mismos como si fuera una de NVIDIA)

------------------------------------------
### **TUTORIAL**:

**1.- Lo primero que tienes que hacer es dirigirte a este [link](https://colab.research.google.com/drive/1go6YwMFe5MX6XM9tv-cnQiSTU50N9EeT?authuser=2) donde podras ver que se nos muestra la pagina de colab donde podrás ver un código hecho en Python como se muestra a continuación.:**
![Imagen 1](https://github.com/OrlandoM117/IA-AprendizajeNoSupervisado-EJEMPLO/blob/master/imagenes/1.png)

**2.- Para configurar nuestro software hecho con NVIDIA-MSI seguiras los pasos siguientes**

- Marcarás en ***Selección de modelos a descargar*** la casilla "imagenet_16384" como se muestra a continuación (Por defecto, el notebook descarga el modelo 16384 de ImageNet. Existen otros que no se descargan por defecto, ya que sería en vano si no los vas a usar, así que si quieres usarlos, simplemente selecciona los modelos a descargar):

![Imagen 2](https://github.com/OrlandoM117/IA-AprendizajeNoSupervisado-EJEMPLO/blob/master/imagenes/2.png)

- Ahora pasamos a la sección de ***Herramientas para la ejecución***. Acá viene lo interesante ya que aqui podremos indicarle al programa si queremos que recreé un video de un "perro" o de un "gato" ya es a gusto del usuario y el número de iteraciones de nuestro video. **Primero** escribimos el objeto o persona que queremos que nuestra IA recreé en el espacio de textos, esto forzosamente tiene que estar escrito en ingles. **Segundo** en el espacio de modelo escojemos el modelo vqgan_imagenet_f16_16384. **Tercero** escribimos el num de iteraciones en el espacio de max_iteraciones, entre más iteraciones pongamos más gráfico se va ver nuestro video y con mayor calidad visual (Entre más iteraciones, más se tarda en procesar) Se recomienda en un rango de 200 a 500 iteraciones.
  
![Imagen 3](https://github.com/OrlandoM117/IA-AprendizajeNoSupervisado-EJEMPLO/blob/master/imagenes/3.png)

- Ahora conectaremos nuestro colab a una maquina virtual con RAM y disco local para poder hacer nuestra ejecución desde el navegador sin utilizar recursos propios.
 
![Imagen 4](https://github.com/OrlandoM117/IA-AprendizajeNoSupervisado-EJEMPLO/blob/master/imagenes/4.png)

- Si quieres utilizar tu tarjeta gráfica dedicada tienes que seleccionar ***"Conectar a un entorno de ejecución local"***
  
![Imagen 5](https://github.com/OrlandoM117/IA-AprendizajeNoSupervisado-EJEMPLO/blob/master/imagenes/5.png)

**3.- Una vez configurado nuestro software de IA y conectado al servidor de colab podemos ejecutar nuestro programa seleccionando el apartado de ***Entorno de ejecución*** y ***Ejecutar Todo***.**

![Imagen 6](https://github.com/OrlandoM117/IA-AprendizajeNoSupervisado-EJEMPLO/blob/master/imagenes/6.png)

**4.- !!LISTO!! ya podrás descargar el video o ver el video desde el navegador. Se vería algo como a continuación como ejemplo escogí la palabra "dog" que significa perro en español**

![Video Dog](https://github.com/OrlandoM117/IA-AprendizajeNoSupervisado-EJEMPLO/blob/master/imagenes/7.png)
