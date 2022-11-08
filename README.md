# Chat-Bidireccional---Sockets---Java

El presente trabajo muestra el diseño e implementación de un chat multicliente bidireccional escrito en Java. Aplica los conceptos básicos de la comunicación por sockets e incluye ciertos requerimientos específicos para su funcionamiento.

Los sockets son un sistema de comunicación entre procesos de diferentes máquinas de una red. Es un punto de comunicación por el cual un proceso puede emitir o recibir información.  
Estos, utilizan una serie de primitivas para establecer el canal de comunicación, para conectarse a una máquina remota en un determinado puerto que esté disponible y así escuchar, leer o escribir y publicar información en él, y desconectarse. Con estos recursos se puede crear un sistema de comunicación completo.

Definición:
Un socket es un punto final en un proceso de comunicación, lo cual permite manejar de una forma sencilla la comunicación entre procesos, aunque estos procesos se encuentren en sistemas distintos, sin necesidad de conocer el funcionamiento de los protocolos de comunicación subyacentes. 

Generalmente, un servidor se ejecuta sobre una computadora específica y tiene un socket que responde en un puerto específico. El servidor únicamente espera, escuchando a través del socket a que un cliente haga una petición.  
Por otro lado, en otra máquina (o para fines demostrativos, en la misma máquina), el cliente conoce el nombre de host de la máquina en la cual el servidor se encuentra ejecutando y el número de puerto en el cual el servidor está conectado. Para realizar una petición de conexión, el cliente intenta encontrar al servidor en la máquina que lo aloje, en el puerto especificado. 

Si todo va bien, el servidor acepta la conexión, se crea un socket adicional con lo cual se crea un hilo o flujo (thread) por cada cliente que se conecte.

Por la parte del cliente, si la conexión es aceptada, un socket se crea de forma satisfactoria 
y puede usarlo para comunicarse con el servidor. Cabe mencionar que el socket 
en el cliente no está utilizando el número de puerto usado para realizar la petición al servidor, sino que este asigna un número de puerto local a la máquina en la cual está 
siendo ejecutado. Ahora el cliente y el servidor pueden comunicarse escribiendo o leyendo en o desde sus respectivos sockets.

La lógica de conexión a través de sockets permite crear aplicaciones de comunicación desde básicas hasta complejas, pues es el principio base de las aplicaciones mas comunes de hoy en día. Este tipo de métodos permite incluso el intercambio de archivos. Es muy interesante ver cómo podemos ampliar este tipo de implementaciones y su potencial.


COMO EJECUTAR LOS ARCHIVOS

SERVER: *Recuerde ejecutar primero el servidor* inicie con

*java Server <port>*
  
 - donde <port> es el puerto que desee utilizar, donde età ubicado el servidor. Si no se establece, se toma por defecto el puerto 1234
  
 CLIENT
  
 *java Client <localhost/IP> <port>*
  
  - donde <localhost/IP> es la IP donde està ubicado el servidor y <port>, el puerto que se asignò previamente en el servidor. Se toma por defecto "localhost" y !1234" respectivamente

  Demostracion: https://www.youtube.com/watch?v=JCEBVKUzr9Q
  
