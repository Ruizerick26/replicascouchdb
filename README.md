# TRABAJO DE ANÁLISIS (RÉPLICAS)
Integrantes: Cataña Dennis, Cocha Iveth, Paredes Miguel, Ruiz Erick y Simba Cristian 

## CREACIÓN DEL SERVIDOR 
Para la creacion del servidor se uso LogMein Hamachi, el cual permitio que las Pc´s se puedan conectar en una misma red. <br>
![image](https://github.com/Ruizerick26/replicascouchdb/assets/117744033/22fc8023-abd0-4641-b05b-7bb4f7202017)

Hamachi nos pide que hamaos login para poder accerder, cuando hagamos login nos aparecera todas las funciones que tiene en su prueba gratis. <br>
![image](https://github.com/Ruizerick26/replicascouchdb/assets/117744033/aeb34d9b-8ba4-4e79-9085-7664ae4892ee)

Para crear la red tenemos que hacer click en la parte superiror de hamachi en la seccion de red.<br>
![image](https://github.com/Ruizerick26/replicascouchdb/assets/117744033/dc91a091-b7df-4cd3-861d-bcb7fdca8eb9)

Una vez ahi presionamos en crear una nueva red Y rellenamos los campos que nos solicita, los cuales son el ID de la red y una contraseña de la misma, y aplastamos en crear. <br>
![image](https://github.com/Ruizerick26/replicascouchdb/assets/117744033/48b8190d-22f8-4efc-a69e-74b66f32e36c)

Y listo tendremos una nueva red creada. <br>
![image](https://github.com/Ruizerick26/replicascouchdb/assets/117744033/b1299400-ce15-48cb-bc10-9da64e2c317c)

Para unirse a una red vamos a ir a la seccion de red y ahora aplastaremos en la opcion de unirse a una red existente.<br>
![image](https://github.com/Ruizerick26/replicascouchdb/assets/117744033/6df500d8-92c4-4062-a995-f2fca57952aa)

Nos pedira las credenciales de una red al completarlas de forma correcta la aplicacion nos unira a la red. 
![image](https://github.com/Ruizerick26/replicascouchdb/assets/117744033/09a6c2db-ad7b-42b8-97cd-2459de071a78)

En esta red a la quenos unimos se podran conectar hasta 5 dispositivos. <br>
![image](https://github.com/Ruizerick26/replicascouchdb/assets/117744033/37b1da9b-147a-45b1-957f-0bde7c7fab3b)

## REPLICA PARA LA RECEPCIÓN DE DATOS
Antes de hacer una réplica, es importante tener en cuenta que se debe desactivar los firewalls para no tener errores.<br><br>
<img width="607" alt="image" src="https://github.com/Ruizerick26/replicascouchdb/assets/117742977/6d905365-57b0-4bc1-9da8-3701d26f3d68"><br><br>
También se debe verificar la conexión entre cliente - servidor con ayuda del comando ping.<br><br>
<img width="899" alt="image" src="https://github.com/Ruizerick26/replicascouchdb/assets/117742977/7c50f13d-9a2c-49f1-bfaf-63785d065cc8">><br><br>
Por otra parte, se crea una base de datos local, la cual con la replica va a recibir la base de datos del servidor.<br><br>
<img width="442" alt="image" src="https://github.com/Ruizerick26/replicascouchdb/assets/117742977/98289506-ea9c-4cd9-90fa-963c8bd202a4"><br><br>
Empezaremos creando la répica, en la parte de source, tendremos que colocar la información del servidor, en esta va las credenciales y la ip del mismo.<br><br>
<img width="485" alt="image" src="https://github.com/Ruizerick26/replicascouchdb/assets/117742977/bd8c83b0-9a4a-4380-bb18-aca1e403b508"><br><br>
En la sección de target, se debe introducir la base local existente que creamos con las credenciales del mismo.<br><br>
<img width="500" alt="image" src="https://github.com/Ruizerick26/replicascouchdb/assets/117742977/96b17c32-e6b6-4c9b-aa95-37a1e32dcf11"><br><br>
En el apartado de option, seleccionaremos que sea de manera continua para que los datos que se envien al servidor lo recepcionemos también.<br><br>
<img width="445" alt="image" src="https://github.com/Ruizerick26/replicascouchdb/assets/117742977/5729619c-6a87-4675-a010-b6717cc45389"><br><br>
Verificamos que la réplica sea existosa.<br><br>
<img width="855" alt="image" src="https://github.com/Ruizerick26/replicascouchdb/assets/117742977/2826b56e-c276-4f61-b202-c509c99eeb75"><br><br>
<img width="850" alt="image" src="https://github.com/Ruizerick26/replicascouchdb/assets/117742977/6a771b92-6b9d-432e-95d5-721923277c97"><br><br>



## REPLICA PARA EL ENVÍO DE DATOS

Seleccionamos nuestra base de datos de la cual vamos a enviar informacion hacia una red remota que ya existe, la opcion de hacer replica se encuentra en el recueadro de doble flecha que se encuentra seleccionado de color rojo<br>
<img width="830" alt="image" src="https://github.com/Ruizerick26/replicascouchdb/assets/117743828/8fda925c-51b5-4cc3-a17a-14b429977683"><br>
LLenamos la informacion sobre la base de datos de origen, que en nuestro caso es una red local<br>
<img width="365" alt="image" src="https://github.com/Ruizerick26/replicascouchdb/assets/117743828/9ebecee1-cce2-49b3-b73b-b25a849732f0"><br>
Volvemos ha hacer lo mismo en la parte de Target, solo que esta vez es con la informacion de la base de destino, que es remota. Volvemos a pedir autentificacion y se deben ingresar el user y la pasword del usuario que creo dicha base<br>
<img width="350" alt="image" src="https://github.com/Ruizerick26/replicascouchdb/assets/117743828/a40bc1e9-9869-4de4-b39d-a15fb2b741aa"><br>
Finalmente seleccionamos el tipo de replica que deseamos, si queremos que los cambios realizados en nuestra base local tambien se efectuen en la base remota (Continuos), o por el contrario que nuestras modificaciones no se relicen en la base remota (one time) <br>
<img width="376" alt="image" src="https://github.com/Ruizerick26/replicascouchdb/assets/117743828/19c1b396-e0b0-4911-80c1-14d15fb49d9c"><br>
Luego se muestra la información sobre nuestra replica, el lugar de origen, lugar de destino, la fecha en la que se realizo, si es continua o no y si se esta efectuando la replica o no <br>
<img width="862" alt="image" src="https://github.com/Ruizerick26/replicascouchdb/assets/117743828/4435c1bd-94de-40fc-8028-6a6bd2cbd499"><br>
## ENVIAR ARCHIVOS A LA BASE DE DATOS
Convertir un archivo CSV a un archivo JSON usando pandas. Los datos JSON se actualizan en la base de datos con campos adicionales como "Nombre" y "Apellido".Finalmente se sube el archivo JSON a una base local
![imagen](https://github.com/Ruizerick26/replicascouchdb/assets/117743367/f78a6fea-7316-4f45-b8de-c61f332090af)
![imagen](https://github.com/Ruizerick26/replicascouchdb/assets/117743367/bd9e67f6-a25e-42ab-ac25-876d691e0699)


## FUNCIÓN DE BÚSQUEDA
Es mejor conocido como  un reporte el cual permite buscar archivos con parametros en específico, para lo cual entraremos a la base de datos y cliquear en Design Documents, y crearemos un nuevo archivo view, el cual permitira crear dicho reporte:<br><br>
![imagen](https://github.com/Ruizerick26/replicascouchdb/assets/117743844/06932df9-b385-4227-848d-3a0097fb14c5)<br><br>
Ahora designaremos un nombre a este reporte y dentro del cuadro de comando agregaremos un condicional, de tal forma solo se mostraran los archivos con el parametro especificado en el condicional:<br><br>
![imagen](https://github.com/Ruizerick26/replicascouchdb/assets/117743844/41ad6a79-b4a9-49ce-bedc-72543238b47a)<br><br>
Ahora se muestra un reporte con un condicional, solicitando que se muestren los archivos con parametro de nombre Erick o apellido Simba:<br><br>
![imagen](https://github.com/Ruizerick26/replicascouchdb/assets/117743844/2c19b271-07dc-46bd-ac0b-9c74b38778d5)<br><br>



