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

---

## **iptraf:** ##
Intercepta paquetes en la red y muestra información sobre el tráfico.

---

## **bandwidthd:** ##
Una herramienta específica de monitorización del ancho de banda
