# Sesión 5 - Ejeccuión


Prueba escrita 2 Marzo

Punto de control de lo que hemos hecho

## Noticia de la semana

https://threatravens.com/france-links-russian-sandworm-hackers-to-hosting-provider-attacks/

[Noticia](https://www.cert.ssi.gouv.fr/cti/CERTFR-2021-CTI-005/)


* __IoC__: Cualquier elemento de información que se puede corresponder con un activo malicioso, url, hash, firma, etc
* [Proyecto](https://www.misp-project.org/) financiado por la Unión Europea
  * SW libre
  * Ligero relativamente
  * manual extraordinario
  * Comunidad que aporta muchísimo, vídeos, etc

* TIP (Threat Intelligence Platform)
* Documentos de francia muy bien explicados, oro puro

## Ejecución

#### Explotación por parte del usuario

### herramientas de despliegue de software

* SCCM

* invoke-expression
  * fileless
* start-process
  * toca disco

### Powershell execution policies
* para los sysadmins si ejecutan algo sin querer
* se puede evadir

### Tareas programadas


### para escalada de privilegios

diskcleanup -> silent cleanup

modificando la variable windir

forzas una nueva tarea programa para abrir una powershell como administrador



### living-off-the land binaries and scripts

abuso de binario y scripts preinstaados en el sistema

https://lolbas-project.github.io


LOLBINS: BITSADMIN

### LOLBINS: Certutil

sentinelone


### Uso de COM/DCOM

COM modelo de objetos distribuidos q cad uno tiene sus funcionaliddes q sean invocados por otros objtos