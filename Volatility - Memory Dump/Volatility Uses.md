Montaje y revisión dumps ram
https://www.seguridadx.com/volatility/

Extraer perfil sistema a montar [Lento. Depende tamaño imagen]
'volatility -f IMAGEN.IMG imageinfo'

Revisar procesos en curso y su pid
'volatility -f IMAGEN.IMG --profile=PERFIL pstree'

Extraer fichero de un proceso
'volatility -f IMAGEN.IMG --profile=PERFIL memdump -p PID -d DIRECTORIODESTINO'

Leer texto de un fichero dumpeado [Default UTF8]
'strings FICHERO > RESULTADO.TXT'
[Se puede variar el numero de bits]
'strings -e l FICHERO > RESULTADO_16BITS.TXT [Para unicode o UTF16]'

Extraer hash contraseñas usuarios windows [Necesario proceso lsass.exe]
'volatility -f IMAGEN.IMG/RAW --profile=PERFIL hasdump'


