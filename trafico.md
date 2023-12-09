## **tcpdump:** ## 
Analiza el tráfico que circula por la red.

```
- tcpdump -i eth0                                      Información sobre una tarjeta de red
- tcpdump -D                                           Ver un listado de las interfaces disponibles para capturar tráfico
- tcpdump -i eth0 -w trafico.log                       Capturar tráfico y enviar a un fichero de texto
- tcpdump -i eth0 [udp,tcp, icmp,...]                  Protocolo a capturar
- tcpdump -i eth0 tcp port 80                          Puerto a capturar
- tcpdump -i eth0 tcp port 80 and src 192.168.1.100    Host o IP de origen
- tcpdump -i eth0 tcp port 80 and dst 192.168.1.100    Host o IP de destino
- tcpdump -i eth0 -A                                   Mostrar el contenido de los paquetes en formato ASCII
- tcpdump -i eth0 -XX                                  Capturar paquetes en hexadecimal y ASCII
- tcpdump -i eth0 not icmp
- tcpdump -i eth0 not icmp and not tcp                 Capturar todo el tráfico excepto ciertas condiciones
- man tcpdump
- tcpdump 'dst 192.168.1.100 and (port http or https)'
- tcpdump -r archivo.log                              Leer captura de tráfico almacenada en un archivo
- 
```
---

## **tcptrack:** ##
Nos muestra las conexiones establecidas, su origen, destino, estado, el tiempo de iddle y la velocidad de transferencia.

```
- tcptrack -i eth0                                              Mostrar todo el tráfico TCP en una interfaz de red-
- tcptrack -i eth0 -t                                           Mostrar el tráfico TCP con información detallada
- tcptrack -i eth0 port 80                                      Filtrar el tráfico por puerto
- tcptrack -i eth0 host 192.168.1.1                             Filtrar el tráfico por dirección IP
- tcptrack -i eth0 -p                                           Mostrar el tráfico en modo promiscuo
- tcptrack -i eth0 port 80 and src host 192.168.1.1             Mostrar tráfico en un puerto y con IP de origen
- tcptrack -i eth0 portrange 8000-9000 and dst host 10.0.0.2    Mostrar tráfico rango de puertos y con IP de destino
- tcptrack -i eth0 src net 192.168.1.0/24 -t                    Filtrar por un rango de direcciones IP de origen y mostrar información detallada
```

---

## **iptraf:** ##
Intercepta paquetes en la red y muestra información sobre el tráfico.

---

## **bandwidthd:** ##
Una herramienta específica de monitorización del ancho de banda
