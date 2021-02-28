# Sesion 4 - Metasploit

## Noticia de la seman

primer hito sobre nuestro escenario

indice y objetivos claros sobre el trabajo grupal

Instalación de la herramienta o leído sobre ella

Estamos listos para comenzar con la interacción con los escenarios

Dudas sobre como orientar los trabajos

Hacker modified drinking water chemical levels in a US city

* Utilizaban mascan, introducido a través de una DLL
  * Más rapido xq implementan su propia pila TCP/IP
  * Introdujeron más dióxido de sodio
  * A través de Team Viewer
  * raidforums, comprar accesos


## Metasploit

Algunos exploits de metasploit están mal a posta, rollo ponen paréntesis y no tira, por que tienes q ver el código y ver donde falla

* burner phone para ir a china


* Código abierto
* Modular
* Extensible
* Core (rex) desacoplado
* Existe Metasploit pro

### Módulos
1. Auxiliary
  * nuca van a generar una sesión
  * conjunto de pruebas pero no genera sesión que interactúe
2. Exploit
3. Payloads
  * Cada una de las piezas de código q quiero ejecutar de una determinada explotación
  * me va a pemitir esa interacción
4. Post
  * Post-expotación, cuando puedo acceder
5. Encoders
  * relacionados con la evasión
  * Evadir distintas medidas
  * orientados a añadir distintas capas de complejidad para evadir los antivirus
  * son diretorios (?)
6. Nops
  * relacionados con la explotación

### Integración con nmap

* odemos usar __db_nmap__
* descubrimiento y vulnerabilidades se pareen a una base de datos de metasploit
  * ver maquina __optimum__ de HTB

### Análisis d vulnerabilidads con metasploit

* Integración con:
  * Nessus
  * OPenVas
  * Nexpose

### Búsqueda de exploits

* `search platform:linux`

* `msfupdate` no existe ya

Para zerologon:
* `apt update; apt install metasploit-framework`
* `apt install ruby2.7 ruby2.7-dev`
* `/usr/share/metasploit-framework$ bundle install`

## Ejemplo explotación básica

* `exploit -j` buscar

* `bind shell` cnexión de cliente a servidor
* `reverse shell` conexión de ervidor a cliente

stdi

## Ejecución manual

1. `searchploit <HFS>`
2. `searchploit -m <num_exploit-db>`


Sesiones

nos permite acceder al cinjunto de funcionanliades que permita abrir una shell remota

cual es el codgio q se ejecuaa en la mquina destino

Interactuamos mediante sesiones

* Información detallada sobre las sesiones
  * `sessiones -v`

* Listado de sesiones
  * `sessions -l`

* Convertir una sesión a meterpreter
  * `sessions -u id_session`

* Interactuar con una sesión
  * `sessions-i id_sesion`



3 tipos de metasploit:
1. Single
2. Staged el nombre la eplotacion requiere varios pasos, q no realizamos nosotros si no las funcionalidades de matasplpot, se consgieu una en el sistma remoto.
   1. `windows/shell/reverse_tcp` 
3. Stageless
   1. PArece lo mismo, diferenciafuncionalidad empotrada en un ejecutable, no a¡hace falta ninguna dll de más, 
   2. `windows/shell_reverse_tcp`

Si yo me uiero abrir una shell con la funcionalidad de una reverse tcp y q engoa como objetic Windows, 

Staged payload

tipo de comun q se establece entre el sistema y el sist remto


modularizar las partes, xq,
* pasar el cinjunt de dlls, estas dlls añaden la funcionalidad q nosotros queremos


Stage 1 o stage 2 en metasploit



* generamos el pauload utilizando __msfvenom__
* Crear __listener__ / __handlers__ en local (multi/handler())
* Desplegamos el payload
* Esperamos a recibir la sesión



Meterpreter payload más famoso, trabaj dentrode l conrtext

migración haia otros procesos, por si alguien cierra el eejeuable q no se corte la conexión q tenga persistencia

Es __fileless__: no ecisten artefacots q residan en el disco dl ordenador
Extensibles

pupy rat

covenant

empire github



cobalt strike

malleable profile

necesitan un c&c,q quieres q haga y pasar cosas, metsploit e un canal cifrado
cobalt dice dime un protocolo e transporte, protocolo de comuncacion del cc, https o http y DNS

por otro lado a q quieres q se parezca, como se camuflan la peticiones (endpoints)

muy famoso el profile de Jquery 

primer profile de cobal q vio enrique es de amazon, busuedas camufladass
