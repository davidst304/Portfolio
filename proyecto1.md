---
layout: default
---
[INICIO](./)
# PROCESOS DE ETL

## **PROYECTO (Extracción reservas, identificación de cambios y envío por telegram).**
**Requerimientos**:

Extracción de manera recurrente las reservas obtenidas duranten el día anterior para que en caso de haber cambios entre la extracción del D-1 con la extración del D se marquen las reservas nuevas en color azul y las reservas con cambios en color verder.
Si entre extracciónes no hay modificación entonces no se tiene que hacer nada.

La tabla resultante con las nuevas reservas y con los cambios se envia por un canal de telegram.

## **Desarrollo.**
1. Conexión y extracción de los datos del aplicativo mediante la API:

    **Herramientas**: Python Requests, Pandas.
2. Comprobación de resultados entre listado D y listado D-1:

    **Herramientas**: Python Pandas.
3. Generación de fichero PDF con los resultados obtenidos:

    **Herramientas**: Python Ironpdf.

4. Adjuntar el fichero pdf y enviarlo por telegram:

    **Herramientas**: Python Requests.

5. Subir el fichero programa al servidor pythonanywhere para el que programa se lanze todos los días a las 6:00 am:

    **Herramientas**: Git y cron.


## **Imagen.**
![Branching](/img/port.jpg)
