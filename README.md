# TareasCursoSeguridad-SCESI [![Logo de la SCESI][logo-SCESI]][enlaceSCESI]
Tareas e investigaciones para postulantes al área seguridad de la SCESI gestión 2024

# Clase 1
## Tarea 1: Laboratorio de Linux Fundamentals
La tarea fue dada durante la primera clase en fecha 21 de mayo.
Solo pude resolver el primer laboratorio debido a que en los otros dos la pagina me mencionaba que era un cuarto premium.
Imagen para comprobación del avance:
<p align="center">
  <img src="https://github.com/SebastianBarreraVargas/TareasCursoSeguridad-SCESI/blob/main/ImagenesGeneral/ImagenesClase1/Tarea1Completada.png" alt="Imagen comprobación avances tarea 1" width="500">
</p>
Imagen para comprobación de que se pide cuartos premium para los cursos 1 y 2:
<p align="center">
  <img src="https://github.com/SebastianBarreraVargas/TareasCursoSeguridad-SCESI/blob/main/ImagenesGeneral/ImagenesClase1/Prueba1.png" alt="Imagen comprobación cuartos premium1" width="700">
</p>
<p align="center">
  <img src="https://github.com/SebastianBarreraVargas/TareasCursoSeguridad-SCESI/blob/main/ImagenesGeneral/ImagenesClase1/Prueba2.png" alt="Imagen comprobación cuartos premium2" width="700">
</p>

## Tarea 2: Laboratorio de HTTP in Detail
En la imagen se puede ver la tarea 100% completa.
<p align="center">
  <img src="https://github.com/SebastianBarreraVargas/TareasCursoSeguridad-SCESI/blob/main/ImagenesGeneral/ImagenesClase1/Tarea2Completada.png" alt="Imagen comprobación cuartos premium2" width="500">
</p>

# Clase 2
## Tarea 3: ¿Qué tipos de NAT existen?
### NAT estatica

La NAT estática es una asignación uno a uno entre una dirección interna y una dirección externa. La NAT estática permite que los dispositivos externos inicien conexiones a los dispositivos internos mediante la dirección pública asignada de forma estática. Por ejemplo, se puede asignar una dirección global interna específica a un servidor web interno de modo que se pueda acceder a este desde redes externas.

### NAT dinámica

El router tiene asignadas varias direcciones IP públicas, de modo que cada dirección IP privada se mapea usando una de las direcciones IP públicas que el router tiene asignadas, de modo que a cada dirección IP privada le corresponde al menos una dirección IP pública. Mientras que la NAT estática proporciona una asignación permanente entre una dirección local interna y una dirección global interna, la NAT dinámica permite la asignación automática de direcciones locales internas a direcciones globales internas.

### NAT de sobrecarga (PAT)

Es el más común de todos los tipos, ya que es el utilizado en los hogares. Se pueden mapear múltiples direcciones IP privadas a través de una dirección IP pública, con lo que evitamos contratar más de una dirección IP pública. Además del ahorro económico, también se ahorran direcciones IPv4, ya que aunque la subred tenga muchas máquinas, todas salen a Internet a través de una misma dirección IP pública.

Para poder hacer esto el router hace uso de los puertos. En los protocolos TCP y UDP se disponen de 65.536 puertos para establecer conexiones. De modo que cuando una máquina quiere establecer una conexión, el router guarda su IP privada y el puerto de origen y los asocia a la IP pública y un puerto al azar. Cuando llega información a este puerto elegido al azar, el router comprueba la tabla y lo reenvía a la IP privada y puerto que correspondan.

## Tarea 4: ¿Como se divide una dirección fisica?

Una dirección fisica se divide de la siguiente manera:
* Los primeros 6 digitos pertenecen al fabricante.
* Los siguientes 6 digitos le pertenecen al dispositivo.

<p align="center">
  <img src="https://github.com/SebastianBarreraVargas/TareasCursoSeguridad-SCESI/blob/main/ImagenesGeneral/ImagenesClase2/ImagenDireccionMAC.png" alt="Imagen direccion MAC" width="500">
</p>

## Tarea 5: Clases de IP

* Clase A: De 10.0.0.0 a 10.255.255.255, que son utilizadas generalmente para grandes redes privadas, por ejemplo de alguna multinacional.

* Clase B: De 172.16.0.0 a 172.31.255.255, que son usadas para redes medianas, como de alguna empresa local, escuela o universidad.

* Clase C: 192.168.0.0 a 192.168.255.255, que son usadas para las redes más pequeñas, como redes domésticas.

* Direcciones IP multicast: Utilizadas para la transmisión de datos a múltiples destinatarios simultáneamente, son esenciales en aplicaciones como transmisiones en vivo y videoconferencias.

Tenemos:

1. Unicast: La comunicación va desde un único origen hasta un destinatario concreto. En este caso, hay un único emisor y receptor, y se utiliza para enviar o recibir datos.

2. Broadcast: Este tipo de comunicación posibilita el envío de datos a todos los usuarios dentro de la misma red local.

3. Anycast: En este tipo de comunicación, la transmisión es de uno a muchos, pero los datos no se envían a todos los receptores, sino solo a los más cercanos. 

<p align="center">
  <img src="https://github.com/SebastianBarreraVargas/TareasCursoSeguridad-SCESI/blob/main/ImagenesGeneral/ImagenesClase2/ClasesDeIP.webp" alt="Imagen Clases de IP" width="500">
</p>

## Tarea 6: ¿Como funciona las tablas ARP en un switch?

ARP es un protocolo de resolución de direcciones, se utiliza para realizar un seguimiento de los dispositivos conectados en el switch. Dentro de este ultimo se tiene la tabla que tiene la dirección IP y MAC de lo que este conectado al SWITCH. Cuando un paquete necesita ser ruteado a un dispositivo determinado, el switch busca la dirección IP del dispositivo en su tabla ARP para obtener la dirección MAC del dispositivo de destino. Nos muestra que dispositivos estan conectados, tambien se puede agregar manualmente dispositivos.

## Tarea 7: ¿Como funciona DHCP?

Es un protocolo que se utiliza para asignar dinamicamente una dirección IP a los dispositivos de forma automatica sin hacer una configuración manual.

Cuando se quiere acceder a una red que usa este protocolo, se le pide una direccion IP y este manda una IP, luego supervisa el uso de la dirección y la recupera después de un tiempo determinado, cuando el dispositivo se apaga o cuando el equipo sale de la red.

## Tarea 8: ¿Como funciona la puerta de enlace predeterminada?

La puerta de enlace predeterminada, o Gateway, es un dispositivo que conecta dos o más redes informáticas. Actúa como un intermediario, guiando el tráfico de datos entre estas redes. Este dispositivo tiene una dirección IP privada y una dirección IP pública. La dirección IP privada se utiliza dentro de la red local, mientras que la dirección IP pública se utiliza para la red exterior.

Basicamente ayuda a conectarse con el exterior.

<p align="center">
  <img src="https://github.com/SebastianBarreraVargas/TareasCursoSeguridad-SCESI/blob/main/ImagenesGeneral/ImagenesClase2/Default-gateway-con-Packet-Tracer.png" alt="Imagen direccion MAC" width="500">
</p>

# Sabado: Primera clase

Se nos pidio realizar las pruebas de la pagina: `https://overthewire.org/wargames/bandit/`

Aqui adjunto las contraseñas actuales de los minijuegos mas una foto de mi terminal en la que terminaba de realizar el nivel 10.

1. `bandit0` (contraseña inicial)

2. `NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL` (contraseña 0-1)

3. `rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi` (contraseña 1-2)

4. `aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG` (contraseña 2-3)

5. `2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe` (contraseña 3-4)

6. `lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR`  (contraseña 4-5)

7. `P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU` (contraseña 5-6)

8. `z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S` (contraseña 6-7)

9. `TESKZC0XvTetK0S9xNwm25STk5iWrBvP` (contraseña 7-8)

10. `EN632PlfYiZbn3PhVK3XOGSlNInNE00t` (contraseña 8-9)

11. `G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s` (contraseña 9-10)

12. `6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM` (contraseña 10-11)

<p align="center">
  <img src="https://github.com/SebastianBarreraVargas/TareasCursoSeguridad-SCESI/blob/main/ImagenesGeneral/Clase1Sabado/Captura_desde_2024-05-31_16-55-40.png" alt="Imagen comprobante nivel 10" width="500">
</p>

La segunda tarea que era en `https://academy.hackthebox.com/module/details/18`
Aqui estan los avances:

<p align="center">
  <img src="https://github.com/SebastianBarreraVargas/TareasCursoSeguridad-SCESI/blob/main/ImagenesGeneral/Clase1Sabado/Captura%20de%20pantalla%202024-05-31%20215046.png" alt="Imagen comprobante hack the box" width="250">
</p>

# Clase 3

## Tarea 9: ¿Que es un ataque DOS?

Un ataque de denegación de servicio (DoS) es un tipo de ciberataque en el que un actor malicioso tiene como objetivo que un ordenador u otro dispositivo no esté disponible para los usuarios a los que va dirigido, interrumpiendo el funcionamiento normal del mismo. Los ataques DoS suelen funcionar al sobrecargar o inundar una máquina objetivo con solicitudes hasta que el tráfico normal es incapaz de ser procesado, lo que provoca una denegación de servicio a los usuarios de la adición. Un ataque DoS se caracteriza por utilizar un único ordenador para lanzar el ataque.

En el caso de los ataques DDoS, se realizan peticiones o conexiones empleando un gran número de ordenadores o direcciones IP. Estas peticiones se realizan todas al mismo tiempo y hacia el mismo servicio objeto del ataque. Un ataque DDoS es más difícil de detectar, ya que el número de peticiones proviene desde diferentes IP´s y el administrador no puede bloquear la IP que está realizando las peticiones, como sí ocurre en el ataque DoS.

Los ordenadores que realizan el ataque DDoS son reclutados mediante la infección de un malware, convirtiéndose así en bots o zombis, capaces de ser controlados de forma remota.

## Tarea 10: ¿Como funcionan los puertos?

Los puertos se utilizan para identificar un terminal de conexión y dirigir datos a un servicio. Hay puertos virtuales y físicos. Los puertos aparecen en la Capa 4, la capa de transporte, del modelo OSI.

Funcionan como puertas de entrada por las que los servidores y máquinas cliente intercambian información. Por ejemplo, un servidor web puede atender simultáneamente las peticiones de páginas web a través del puerto 80 para HTTP y del puerto 443 para HTTPS, mientras un cliente de correo electrónico puede recibir e-mails a través del puerto 993.

<p align="center">
  <img src="https://github.com/SebastianBarreraVargas/TareasCursoSeguridad-SCESI/blob/main/ImagenesGeneral/ImagenesClase3/comunicacion-con-puertos.png" alt="Imagen comprobante hack the box" width="500">
</p>

## Tarea 11: ¿Cuantos puertos existen?

Hay 65536 puertos aunque no todos se llegan a usar.

## Tarea 12: Tipos de puertos

* Puertos conocidos: los puertos conocidos (well-known en inglés) van desde el puerto 0 hasta al 1023, están registrados y asignados por la Autoridad de Números Asignados de Internet (IANA). Por ejemplo, en este listado de puertos está el puerto 20 de FTP-Datos, el puerto 21 de FTP-Control, el puerto 22 de SSH, puerto 23 de Telnet, puerto 80 y 443 para web (HTTP y HTTPS respectivamente), y también el puerto de correo entre otros muchos protocolos de la capa de aplicación.
* Puertos registrados: los puertos registrados van desde el puerto 1024 hasta al 49151. La principal diferencia de estos puertos, es que las diferentes organizaciones pueden hacer solicitudes a la IANA para que se le otorgue un determinado puerto por defecto, y se le asignará para su uso con una aplicación en concreto. Estos puertos registrados están reservados, y ninguna otra organización podrá registrarlos nuevamente, no obstante, normalmente están como «semireservados», porque si la organización deja de utilizarlo podrá reutilizarse por otra empresa. Un claro ejemplo de puerto registrado es el 3389, se utiliza para las conexiones RDP de Escritorio Remoto en Windows.
* Puertos efímeros: estos puertos van desde el 49152 hasta el 65535, este rango de puertos se utiliza por los programas del cliente, y están constantemente reutilizándose. Este rango de puertos normalmente se utiliza cuando está transmitiendo a un puerto conocido o reservado desde otro dispositivo, como en el caso de web o FTP pasivo. Por ejemplo, cuando nosotros visitamos una web, el puerto de destino siempre será el 80 o el 443, pero el puerto de origen (para que los datos sepan cómo volver) hace uso de un puerto efímero.

## Tarea 13: ¿Que es Docker?

Es una plataforma de software que te permite crear, probar e implementar aplicaciones de manera sencilla en contenedores. Estos contenedores son como máquinas virtuales muy livianas, lo que te da la flexibilidad de crear, implementar, copiar y mover tus aplicaciones de un entorno a otro, optimizando así las aplicaciones para la nube.

Docker utiliza el kernel de Linux y sus funciones para dividir los procesos y ejecutarlos de manera independiente. Esto permite que varias aplicaciones funcionen en diferentes entornos complejos. Por ejemplo, Docker te permite ejecutar el sistema de gestión de contenidos WordPress en sistemas Windows, Linux y macOS sin ningún problema.

Los contenedores Docker comparten el sistema operativo del anfitrión, mientras que las máquinas virtuales tienen un sistema operativo invitado que se ejecuta sobre el sistema anfitrión.

# Clase 4

## Tarea 14: Diferencia entre PUT y POST

* `PUT`: Este actualiza lo que esta disponible en el servidor, reemplaza lo que esta en la URL por otra cosa. Puede sobreescribir y es idemponente (el resultado no cambia sin importar cuantas veces lo envies).
* `POST`: Este a diferencia de `PUT` no es idemponente lo cual genera que al enviarlo mas veces pueda tener efectos adicionales.

<details>
    <summary> Abreme para ver la explicación de un ejemplo  :exclamation: :exclamation:</summary>
  
Imagina que estás utilizando el método POST para enviar un formulario de registro en un sitio web. Cada vez que envías el formulario, se crea una nueva cuenta de usuario. Si envías el mismo formulario dos veces, se crean dos cuentas de usuario diferentes, aunque los datos del formulario sean los mismos. Esto es porque el método POST está diseñado para enviar y procesar datos, pero no para reemplazar o actualizar datos existentes.

Peroooo, si utilizas el método PUT para actualizar la información de un usuario existente y envías la misma solicitud varias veces, la información del usuario no cambiará después de la primera solicitud, porque PUT es idempotente y está diseñado para actualizar datos existentes.

</details>

[logo-SCESI]: https://github.com/SebastianBarreraVargas/Git/blob/main/Imagenes/scesi-para-fondo-claro-1.png
[enlaceSCESI]: https://www.scesi.org