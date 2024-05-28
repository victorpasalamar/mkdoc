# Documentació Projecte FOG amb MKDocs

Aquest es el meu ficher mkdocs amb el que fare la documentacio de la instal·lacio, configuració i funcionament del meu servidor FOG

## Instal·lacio

Primer que tot a la maquina servidor li posem un adaptador en mode pont i un amb red interna
![Texto alternativo](images/1.png) 
![Texto alternativo](images/2.png)

Configurem la red interna per a que la IP sigui estatica

![Texto alternativo](images/3.png)

Quan tinguem la red ben feta descarregem el fog de la pagina oficial

![Texto alternativo](images/4.png)

Llavors descomprimim l’arxiu

![Texto alternativo](images/5.png)
![Texto alternativo](images/6.png)

Com utilitzem ubuntu, la opcio que hem de escollir es la dos:

![Texto alternativo](images/7.png)

Seleccionarem el tipus d'instal·lació normal, canviarem la interfície de xarxa per defecte per la nova que hem configurat i li indicarem com a DHCP la direcció de la nostra xarxa interna.

![Texto alternativo](images/8.png)
![Texto alternativo](images/9.png)

Confirmem que tot el que hem seleccionat es correcte i continuem

![Texto alternativo](images/10.png)

Despres de tota la instal·lacio ens sortira on hem de anar per a entrar de forma grafica:

![Texto alternativo](images/11.png)

Completem la instal·lacio desde l’adreça

![Texto alternativo](images/12.png)

Despres de la instal·lacio web podem premer enter a la terminal per a acabar la instal·lacio del fog desde terminal

![Texto alternativo](images/13.png)

Despres de la instal·lacio ens donara les credencials per a poder entrar al fog

![Texto alternativo](images/14.png)

Accedim al fog:

![Texto alternativo](images/15.png)
![Texto alternativo](images/16.png)
## Creacio de imatges
El que farem a continuacio sera crear les imatges windows:

![Texto alternativo](images/17.png)

Per a la de windows al apartat de Image Type seleccionarem Multiple Partition Image Single
Disk.

![Texto alternativo](images/18.png)

Afegim el client windows desde hosts i create new hosts

![Texto alternativo](images/19.png)
![Texto alternativo](images/20.png)

Despres d’aixo a List All hosts podem veure la maquina que hem creat
Llavors farem clic a la incona groga per a que ens fase la copia de la imatge del windows

![Texto alternativo](images/21.png)
![Texto alternativo](images/22.png)
![Texto alternativo](images/23.png)

Ara farem el mateix pero amb un Ubuntu

![Texto alternativo](images/24.png)
![Texto alternativo](images/25.png)
![Texto alternativo](images/26.png)
![Texto alternativo](images/27.png)
##Captura de client windows
Ara iniciarem la maquina windows

![Texto alternativo](images/28.png)

Entrarem en mode LAN

![Texto alternativo](images/29.png)
![Texto alternativo](images/30.png)

Despres de la carga de la imatge windows podem comprobar com s’ha pasat correctament al veure quan pesa la imatge del windows 10

![Texto alternativo](images/31.png)

##Captura de client ubuntu

![Texto alternativo](images/32.png)

Farem com en windows i entrarem en mode lan per a pujar la imatge del ubuntu

![Texto alternativo](images/33.png)

##Instalar imatge windows

Per a instalar la imatge agafem una maquina verge (sense iso) i entrem en mode lan per a que obrigue el fog
![Texto alternativo](images/34.png)

Pero abans de iniciar-la es important recordar posar la red en interna i registrar la maquina com a host

![Texto alternativo](images/35.png)
![Texto alternativo](images/36.png)
![Texto alternativo](images/37.png)

Anem a l’opcio de deploy image per a pasar-li la imatge del windows 10

![Texto alternativo](images/38.png)
![Texto alternativo](images/39.png)

I instalem el windows 10

![Texto alternativo](images/40.png)
![Texto alternativo](images/41.png)
![Texto alternativo](images/42.png)

Aqui es pot veure com son les mateixes maquines despres de la instalacio amb la imatge

![Texto alternativo](images/43.png)

##Llançar un paquet d'instal·lacio als clients
Primer el que haurem de fer per al windows es instalar el client de fog

![Texto alternativo](images/44.png)
![Texto alternativo](images/45.png)
![Texto alternativo](images/46.png)
![Texto alternativo](images/47.png)
![Texto alternativo](images/48.png)
![Texto alternativo](images/49.png)

Comprobem que esta en execucio el servei

![Texto alternativo](images/50.png)

Instalem el paquet al servidor i creem l’Snapin

![Texto alternativo](images/51.png)

Entrem dins del client desde el fog i dins dels snapins anyadirem el que acabem de crear

![Texto alternativo](images/52.png)

Despres anem a tasques i single snapin

![Texto alternativo](images/53.png)

Llavors seleccionem el snapin i li donem a task

![Texto alternativo](images/54.png)
![Texto alternativo](images/55.png)

Llavors hem de anar a tasques i esperar

![Texto alternativo](images/56.png)

M’he adonat de que esta fent alguna cosa extranya, perque en teoria esta instal·lant el mozila firefox de forma correcta pero no veig que s’instali a la maquina client

![Texto alternativo](images/57.png)
![Texto alternativo](images/58.png)

