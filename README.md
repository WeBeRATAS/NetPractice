# NetPractice
NetPractice 42

¡Hola! Prepárate para sumergirte en el mundo de las redes como un auténtico estudiante de 42. Aquí tienes tu guía NetPractice, explicada de forma sencilla y directa:

**NetPractice: Tu Aventura en el Mundo de las Redes**

Imagina que NetPractice es como un videojuego donde, en lugar de controlar a un personaje, controlas la información que viaja por internet. Aprenderás a configurar, entender y solucionar problemas de redes, ¡como un verdadero mago de la tecnología!

**Principios Fundamentales (¡Las Reglas del Juego!)**

1.  **Modelo OSI: El Alfabeto de las Redes**

    *   Piensa en el modelo OSI como un edificio de 7 pisos. Cada piso (capa) tiene una función específica en el proceso de comunicación.
    *   La información (un mensaje, una foto, un video) baja por estos pisos, añadiendo "etiquetas" en cada uno, como si se preparara para un viaje.
    *   Cuando llega al destino, sube por los mismos pisos, quitándose las "etiquetas" hasta que el mensaje original llega a la aplicación.
    *   **Las 7 capas:**
        1.  **Física:** Cables, señales de radio... ¡lo tangible!
        2.  **Enlace de datos:** Organiza los datos en "paquetes" (tramas) y los envía al siguiente punto.
        3.  **Red:** Decide la ruta (como un GPS) para que los paquetes lleguen a su destino.
        4.  **Transporte:** Asegura que los datos lleguen completos y en orden (como un servicio de mensajería confiable).
        5.  **Sesión:** Abre y cierra la comunicación entre aplicaciones (como una llamada telefónica).
        6.  **Presentación:** Traduce los datos para que las aplicaciones los entiendan (como un intérprete).
        7.  **Aplicación:** ¡Donde ocurre la magia! Aquí están tus apps favoritas: navegadores, correo, etc.

2.  **Protocolos: Los Idiomas de Internet**

    *   Los protocolos son como idiomas que usan las computadoras para hablar entre sí.
    *   **TCP/IP:** Es el idioma principal de internet (como el inglés).
        *   **TCP:** Es como enviar una carta certificada. Se asegura de que todo llegue y en orden.
        *   **IP:** Es como la dirección postal. Indica a dónde debe ir la información.
    *   **UDP:** Es como enviar una postal. Es más rápido, pero no se garantiza que llegue todo.
    *   **HTTP/HTTPS:** Para navegar por la web (como pedir comida a domicilio).
    *   **FTP:** Para transferir archivos (como enviar un paquete por correo).
    *   **SSH:** Para controlar otra computadora de forma segura (como usar un control remoto).
    *   **DNS:** El "directorio telefónico" de internet. Traduce nombres de dominio (como google.com) a direcciones IP.

3.  **Direcciones IP: La Identidad de Cada Dispositivo**

    *   Cada dispositivo conectado a internet tiene una dirección IP, como su número de identificación.
    *   **IPv4:** Es como un número de teléfono antiguo (ej: 192.168.1.1).
    *   **IPv6:** Es como un número de teléfono moderno, con más espacio para todos (ej: 2001:0db8:85a3:0000:0000:8a2e:0370:7334).
    *   **Máscara de subred:** Indica qué parte de la dirección IP es la red y qué parte es el dispositivo.

4.  **Puertos: Las Puertas de Entrada a las Aplicaciones**

    *   Los puertos son como puertas numeradas en una casa. Cada aplicación usa un puerto específico para comunicarse.
    *   Ejemplos:
        *   Puerto 80: HTTP (web)
        *   Puerto 443: HTTPS (web segura)
        *   Puerto 22: SSH (control remoto seguro)

**Ejercicios NetPractice: ¡Manos a la Obra!**

1.  **Configuración de Redes:**

    *   Aprenderás a asignar direcciones IP, máscaras de subred y puertas de enlace a tus dispositivos.
    *   Configurarás routers y switches (¡como los semáforos de internet!).
    *   Crearás redes locales (LAN) y conectarás diferentes redes entre sí.
    *   Utilizarás herramientas como `ifconfig` (o `ipconfig` en Windows) para ver la configuración de red de tu máquina.

2.  **Resolución de Problemas (Troubleshooting):**

    *   Serás como un detective de redes, buscando pistas para resolver problemas.
    *   Usarás herramientas como:
        *   `ping`: Para ver si puedes comunicarte con otro dispositivo.
        *   `traceroute` (o `tracert` en Windows): Para ver la ruta que siguen los paquetes.
        *   `nslookup`: Para consultar información de DNS.
        *   `netstat`: Para ver las conexiones de red activas.
        *   `tcpdump` o Wireshark: Para "espiar" el tráfico de red y ver qué está pasando (¡como un microscopio!).

3.  **Simulación de Redes:**

    *   Usarás software como GNS3 o Cisco Packet Tracer para crear redes virtuales y experimentar sin riesgos.
    *   Podrás diseñar y probar diferentes escenarios de red.

**Consejos de Supervivencia**

*   **¡No te rindas!** La red puede ser compleja, pero con paciencia y práctica, lo dominarás.
*   **Pregunta, investiga, experimenta.** La comunidad de 42 y la internet están llenas de recursos.
*   **Divide y vencerás.** Los problemas grandes se resuelven mejor en partes pequeñas.
*   **Dibuja diagramas.** Te ayudará a visualizar la red y entender cómo funciona.
*   **¡Diviértete!** Aprender sobre redes es como descubrir un nuevo mundo.

# Ejemplo de Escenario

Supongamos que te dan la siguiente información:

Dirección de red: 192.168.10.0
Máscara de subred: 255.255.255.0 (/24)
Requisitos de subredes:
Subred A: 60 hosts
Subred B: 28 hosts
Subred C: 12 hosts
Subred D: 12 hosts
La Lógica: Direcciones IP y Máscaras de Subred

Antes de sumergirnos en la solución, repasemos la lógica fundamental:

Dirección IP: Una dirección IPv4 se compone de 32 bits, divididos en cuatro octetos (grupos de 8 bits). Cada octeto se representa en decimal (0-255). Ejemplo: 192.168.10.0
Máscara de Subred: También tiene 32 bits. Los bits "1" en la máscara indican la parte de la dirección IP que pertenece a la red. Los bits "0" indican la parte que pertenece a los hosts (dispositivos).
Prefijo de Red (Notación CIDR): La notación /24 es una forma abreviada de escribir la máscara 255.255.255.0. El número después de la barra (/) indica cuántos bits "1" hay en la máscara.
Visualización: Bits y Octetos

code.txt
Copy
Download
Dirección IP:  192      . 168      . 10       . 0
               11000000 . 10101000 . 00001010 . 00000000

Máscara (/24): 255      . 255      . 255      . 0
               11111111 . 11111111 . 11111111 . 00000000
               --------   --------   --------   --------
               Red        Red        Red        Host (8 bits para hosts)
En este caso (/24), los primeros 24 bits son para la red, y los últimos 8 bits son para los hosts. Esto significa que tenemos 28 = 256 direcciones posibles en esta red. Pero, ¡cuidado! No todas son utilizables:

Dirección de Red: La primera dirección (todos los bits de host en 0) se reserva para identificar la red misma (192.168.10.0).
Dirección de Broadcast: La última dirección (todos los bits de host en 1) se usa para enviar mensajes a todos los dispositivos de la red (192.168.10.255).
Por lo tanto, tenemos 256 - 2 = 254 direcciones de host utilizables.

Pasos para la Solución (Subnetting)

Ordenar los Requisitos: Ordena las subredes de mayor a menor según la cantidad de hosts necesarios: A (60), B (28), C (12), D (12).

Calcular la Máscara de Subred Necesaria (para cada subred):

Subred A (60 hosts):

Necesitamos encontrar la potencia de 2 más cercana (y mayor o igual) al número de hosts más 2 (dirección de red y broadcast). 60 + 2 = 62.
26 = 64. Esto es suficiente. Necesitamos 6 bits para hosts.
Si necesitamos 6 bits para hosts, y una dirección IP tiene 32 bits, entonces 32 - 6 = 26 bits son para la red.
La máscara de subred será /26 (255.255.255.192).
Subred B (28 hosts):

28 + 2 = 30
25 = 32. Necesitamos 5 bits para hosts.
32 - 5 = 27 bits para la red.
Máscara: /27 (255.255.255.224).
Subred C (12 hosts):

12 + 2 = 14
24 = 16. Necesitamos 4 bits para hosts.
32 - 4 = 28 bits para la red.
Máscara: /28 (255.255.255.240).
Subred D (12 hosts):

Igual que Subred C: /28 (255.255.255.240).
Asignar Direcciones de Red (a cada subred):

Subred A (/26):

Comenzamos con la dirección de red original: 192.168.10.0
Dirección de red: 192.168.10.0
Dirección de broadcast: 192.168.10.63 (los últimos 6 bits en 1)
Rango de hosts utilizables: 192.168.10.1 - 192.168.10.62
Subred B (/27):

La siguiente dirección disponible después de la subred A es 192.168.10.64
Dirección de red: 192.168.10.64
Dirección de broadcast: 192.168.10.95 (los últimos 5 bits en 1, partiendo de .64)
Rango de hosts utilizables: 192.168.10.65 - 192.168.10.94
Subred C (/28):

Siguiente dirección: 192.168.10.96
Dirección de red: 192.168.10.96
Dirección de broadcast: 192.168.10.111
Rango de hosts utilizables: 192.168.10.97 - 192.168.10.110
Subred D (/28):

Siguiente dirección: 192.168.10.112
Dirección de red: 192.168.10.112
Dirección de broadcast: 192.168.10.127
Rango de hosts utilizables: 192.168.10.113 - 192.168.10.126
Tabla Resumen

Subred	Requisitos	Máscara (CIDR)	Máscara (Decimal)	Dirección de Red	Rango de Hosts Utilizables	Broadcast
A	60 hosts	/26	255.255.255.192	192.168.10.0	192.168.10.1 - 192.168.10.62	192.168.10.63
B	28 hosts	/27	255.255.255.224	192.168.10.64	192.168.10.65 - 192.168.10.94	192.168.10.95
C	12 hosts	/28	255.255.255.240	192.168.10.96	192.168.10.97 - 192.168.10.110	192.168.10.111
D	12 hosts	/28	255.255.255.240	192.168.10.112	192.168.10.113 - 192.168.10.126	192.168.10.127

# Ejemplo de desarrollo de una red: 192.168.10.0/24 (Red Original)

├── 192.168.10.0/26 (Subred A)  [0-63]
│   ├── 192.168.10.0   (Dirección de red)
│   ├── 192.168.10.1-62 (Hosts)
│   └── 192.168.10.63  (Broadcast)


│
├── 192.168.10.64/27 (Subred B) [64-95]
│   ├── 192.168.10.64  (Dirección de red)
│   ├── 192.168.10.65-94 (Hosts)
│   └── 192.168.10.95  (Broadcast)



│
├── 192.168.10.96/28 (Subred C) [96-111]
│   ├── 192.168.10.96  (Dirección de red)
│   ├── 192.168.10.97-110 (Hosts)
│   └── 192.168.10.111 (Broadcast)



│
└── 192.168.10.112/28 (Subred D) [112-127]
    ├── 192.168.10.112 (Dirección de red)
    ├── 192.168.10.113-126 (Hosts)
    └── 192.168.10.127 (Broadcast)


    


# Explicación Adicional (Máscaras en Binario)

Para entender completamente por qué las máscaras son como son, veamos su representación binaria:

/26: 255.255.255.192 -> 11111111.11111111.11111111.11000000 (26 unos, 6 ceros)
/27: 255.255.255.224 -> 11111111.11111111.11111111.11100000 (27 unos, 5 ceros)
/28: 255.255.255.240 -> 11111111.11111111.11111111.11110000 (28 unos, 4 ceros)
Los "unos" a la izquierda "enmascaran" la parte de la red, y los "ceros" a la derecha son el espacio para las direcciones de host dentro de cada subred. Al "mover" los "unos" hacia la derecha, creamos subredes más pequeñas con menos hosts disponibles.

# Puntos Clave

Siempre +2: Recuerda siempre sumar 2 al número de hosts requeridos para tener en cuenta la dirección de red y la de broadcast.
Potencias de 2: La cantidad de hosts utilizables en una subred (sin contar red y broadcast) siempre será una potencia de 2 menos 2.
Orden Descendente: Asigna primero las subredes más grandes. Esto evita la fragmentación y facilita la administración.
Visualiza en Binario: Si te sientes confundido, convierte las direcciones y máscaras a binario. Te ayudará a ver cómo se dividen los bits.

