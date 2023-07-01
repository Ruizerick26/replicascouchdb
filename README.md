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


## ENVIAR ARCHIVOS A LA BASE DE DATOS

## FUNCIÓN DE BÚSQUEDA
