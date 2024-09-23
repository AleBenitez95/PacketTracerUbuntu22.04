# PacketTracerUbuntu22.04

## Error instalación Packet Tracer por el paquete libgl1-mesa-glx

```
1asir@pc119:~/Descargas$ sudo apt-get install ./Packet_Tracer822_amd64_signed.deb 
Leyendo lista de paquetes... Hecho
Creando árbol de dependencias... Hecho
Leyendo la información de estado... Hecho
Nota, seleccionando «packettracer» en lugar de «./Packet_Tracer822_amd64_signed.deb»
No se pudieron instalar algunos paquetes. Esto puede significar que
usted pidió una situación imposible o, si está usando la distribución
inestable, que algunos paquetes necesarios aún no se han creado o se
han sacado de «Incoming».
La siguiente información puede ayudar a resolver la situación:

Los siguientes paquetes tienen dependencias incumplidas:
 packettracer : Depende: libgl1-mesa-glx pero no es instalable
E: No se pudieron corregir los problemas, usted ha retenido paquetes rotos.

```
Para resolver esto descargamos el segundo paquete de este repositorio:

https://github.com/PetrusNoleto/Error-in-install-cisco-packet-tracer-in-ubuntu-23.10-unmet-dependencies/releases/download/CiscoPacketTracerFixUnmetDependenciesUbuntu23.10/libgl1-mesa-glx_23.0.4-0ubuntu1.22.04.1_amd64.deb

Luego hacemos el comando:

```
sudo dpkg -i libgl1-mesa-glx_23.0.4-0ubuntu1.22.04.1_amd64.deb

```
Una vez hecho esto ya puedes instalar Pakcet Tracer con el siguiente comando:

```
sudo apt-get install ./Packet_Tracer822_amd64_signed.deb
```

