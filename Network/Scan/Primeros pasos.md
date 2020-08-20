* Recomendado Kali

1. Footprinting
TheHarvester.
Recolectar información de terceros (internet)

`theharvester -d DOMINIO -l NUMERO_RESULTADOS -b (BUSCADOR/all)`

* Nos ofrece subdominios, correos disponibles y servidores actuales.

2. Fingerprinting -> Interactuar con la victima.
Utilizando los datos anteriores, !!consultar en shodan desde IP (theharvester)!!

Banner Grabbing -> Descubrimiento de versiones de los servicios del servidor a través de banners y cabeceras de las peticiones hacia los puertos identificados.
 * Netcat `nc IP PUERTO`
 * Telnet `telnet IP PUERTO`
* Ping (tcp 7) `ping IP`
* Nmap `nmap -sV [-sC] [-o FicheroSalida] -p (PUERTO/RANGO) IP --script=banner`  -> si ejecutamos como root, permite utilizar un solo handshake para todo el escaneo de la misma IP dest.

** En caso de ping bloqueado, la opción -sV permite evitar la consulta y ejecutar el escaneo forzado. **

** opción -sC ejecuta todos los scripts disponibles. Portal scripts oficiales disponibles <https://nmap.org/nsedoc/>

*** La respuesta devuelve la informacion del puerto ***

**Util maquina metaexploitable
<https://sourceforge.net/projects/metasploitable/files/latest/download>


3. Análisis de vulnerabilidades
   CVSS -> Common Vulnerability Scoring System

   Identificar vulnerabilidades 
   Diccionario <https://nvd.nist.gov/>
   Detalles Vulnerabilidad <https://www.cvedetails.com/>
   Open Sourced Vulnerability Database (OSVDB) <>
   CVE -> Common Vulnerabilities and Exposure. Estado de un sistema que permite:
    * Ejecutar comandos como otro usuario
    * Acceso a datos violando las restricciones de acceso
    * Suplantar otra identidad
    * Ejecutar denegación de servicio

   BID (BugTraq ID). Vulnerabilidad reportada por Symantec.

   Buscador exploits y soluciones a las vulnerabilidades <https://www.securityfocus.com/>

   MS (Microsoft Security). Vulnerabilidades y actualizaciones de seguridad en sistemas Windows <https://support.microsoft.com/es-es/>

