# AZURE - CHATBOT
**En esta practica aprenderas a crear un chatbot con azure desde la pagina de qnamaker**

## Requisitos
- Tener una suscripcion en Azure
- Tener una conexion a internet
- Tener un navegador instalado (Brave,Google,Firefox, etc)

-------------------------

## TUTORIAL

**1.-Primero nos vamos a [Qnamaker](https://www.qnamaker.ai/) y le damos en "Create a knowledge base"**

![imagen 1](imagenes/1.png)

**2.-Ahora le damos en "Create a Qna Service"**

![imagen 2](imagenes/2.png)

**3.-Le damos lo minimo que se ocupa para crear un recurso de azure (puedes agarrar esta configuracion como ejemplo) y le damos en revisar y crear**

![imagen 3](imagenes/3.png)

**4.-Ahora en el STEP 2 le damos un directorio, una suscripcion, el qna Service que acabamos de crear, el lenguaje del bot, y en STEP 3 le damos el nombre de de la referencia del bot**

![imagen 4](imagenes/4.png)

**5.-Ahora en el STEP 4 en "Chit Chat" podemos seleccionar cual es la personalidad del bot en este caso va ser (Amigable) en Populate your KB (puedes extraer la pregunta y respuesta desde tu base de datos o desde una url)**

![imagen 5](imagenes/5.png)

***6.-Y por ultimo en STEP 5, le damos en Create your KB**

![imagen 6](imagenes/6.png)

**7.-Ahora nos mandará a esta pagina donde podremos ir baseando nuestras preguntas y respuestas del chatbot**

![imagen 7](imagenes/7.png)

**8.-Le podremos dar en la opcion de "Add QNA " para agregar nuestra pregunta y respuesta**

![imagen 8](imagenes/8.png)

**9.-Si le damos en test podemos probar al bot**

![imagen 9](imagenes/9.png)

**10.-Una vez terminado nuestro bot, le damos en save and train**

![imagen 10](imagenes/10.png)

**11.-Una vez entrenado le daremos en publish**

![imagen 11](imagenes/11.png)

**12.-Una vez hecho podemos ó copiar el Postman para pegarlo en nuestro codigo de pagina ó darle en "Create Bot" para poder hacerlo desde azure y conectarlo a una extension**

![imagen 12](imagenes/12.png)

**13.-Nos mandar a crear un recurso para hacer un Web App Bot , donde le damos lo minimo para crear un recurso (puedes usar esta configuracion)**

![imagen 13](imagenes/13.png)

**14.-Como puedes ver ya esta creado el bot donde le puedes dar en Appy para aplicar la descripcion y/o el nombre**

![imagen 14s](imagenes/14.png)

**15.-Podemos hacer un test, vamos al apartado "Test in Web Chat" y le mandamos algo**

![imagen 15](imagenes/15.png)

**16.-Ahora para poder conectarlo desde azure, nos vamos a Channels y podemos seleccionar cualquiera de estos (en esta practica será teams)**

![imagen 16](imagenes/16.png)

**17.-Aplicamos la configuracion y le daremos en Apply**

![imagen 17](imagenes/17.png)

**18.-Una vez hecho esto , ahora podremos ver que nuestro bot esta conectado desde Microsoft teams y lo podemos abrir**

![imagen 18](imagenes/18.png)

**19.-Como test podrás ver que ahora funciona**

![imagen 19](imagenes/19.png)