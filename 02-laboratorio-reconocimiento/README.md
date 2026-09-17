Proyecto 2 - Laboratorio en etapa de reconocimiento del adversario

En este laboratorio, utilicé comandos, herramientas y documenté los pasos en una etapa de reconocimiento del adversario, dentro de una máquina virtual en la plataforma de HackTheBox, entendiendo el paso a paso del comienzo de un posible ataque, para poder así, entender y darme cuenta en caso de que se produzca, y poder mitigar el ataque antes de que produzca desastres.

Qué hice:

En primer lugar, me conecté mediante una VPN, a la máquina virtual de HackTheBox, verifiqué que la conexión estuviera estable desde la terminal de Windows con el comando de IPCONFIG, una vez verificada la conexión, procedí con la etapa de reconocimiento, tirando un PING a la IP de destino que me había otorgado la plataforma. 

Fui continuando los pasos de la etapa y utilizando comandos Y Parámetros de la herramienta Nmap, para verificar que puertos y servicios habían abiertos.

Por ejemplo:

Nmap -sc -sV <IP>  (para escanear si hay puertos abiertos y obtener información de las versiones de servicios que se ejecutan en estos puertos)

Descubrimos que el puerto 23 TELNET estaba abierto, y utilizamos los comandos como:

telnet <IP>

pero al descubrir que nos pedía credenciales, decidí utilizar los siguientes parámetros:

telnet -l root <IP>

objetivo cumplido: pudimos acceder a la máquina Linux con permiso de administrador, utilizamos el comando:

ls para listar los directorios, y el comando cat sobre el archivo de texto plano flag.txt para poder capturar la bandera.

