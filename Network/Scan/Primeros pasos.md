* Recomendado Kali

1. Footprinting
TheHarvester.
Recolectar información de terceros (internet)

`theharvester -d DOMINIO -l NUMERO RESULTADOS -b (BUSCADOR/all)`

* Nos ofrece subdominios, correos disponibles y servidores actuales.

2. Fingerprinting -> Interactuar con la victima.
Utilizando los datos anteriores, consultar en shodan

Banner Grabbing -> Descubrimiento de versiones de los servicios del servidor a través de banners y cabeceras de las peticiones hacia los puertos identificados.
 * Netcat `nc IP PUERTO`
 * Telnet `telnet IP PUERTO`
 * Nmap `nmap -sV -p PUERTO IP --script=banner`

