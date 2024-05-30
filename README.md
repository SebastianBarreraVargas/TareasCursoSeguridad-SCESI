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
  <img src="" alt="Imagen direccion MAC" width="500">
</p>


[logo-SCESI]: https://github.com/SebastianBarreraVargas/Git/blob/main/Imagenes/scesi-para-fondo-claro-1.png
[enlaceSCESI]: https://www.scesi.org