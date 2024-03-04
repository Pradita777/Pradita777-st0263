# info de la materia: STxxxx <nombre>
#
# Estudiante(s): Andres Prada Rodriguez, apradar@eafit.edu.co
#
# Profesor: Edwin Nelson Montoya Munera, emontoya@eafit.edu.co
#

# Reto 1 y 2 Conexión pear to pear
#
# 1. breve descripción de la actividad
#
<La idea del proyecto es crear una red pear to pear con un servidor central, esto para que cada pear carge o descargue archivos.>
## 1.1. Que aspectos cumplió o desarrolló de la actividad propuesta por el profesor (requerimientos funcionales y no funcionales)
### Cumpli con crear el servidor central, el pserver y el pclient, la comunicacion entre el pserver y el servidor central, montar a docker el servidor central y montarlo a una instancia de aws, que al conectarse con el pserver lo agregara a su lista.
## 1.2. Que aspectos NO cumplió o desarrolló de la actividad propuesta por el profesor (requerimientos funcionales y no funcionales)
No logre conectar el pclient con otro pserver para el download de archivos, no logre el logout del servidor central, no logre montar a docker el pserver y el pclient, como tampoco los monte a aws.
# 2. información general de diseño de alto nivel, arquitectura, patrones, mejores prácticas utilizadas.
## El diseño de alto nivel del proyecto se basa en una arquitectura cliente-servidor distribuida, donde el servidor central actúa como punto centralizado de coordinación y los pares gestionan el almacenamiento y distribución de archivos.
# 3. Descripción del ambiente de desarrollo y técnico: lenguaje de programación, librerias, paquetes, etc, con sus numeros de versiones.
## Python 3.12.2 
## Requistos: grpcio grpcio-tools fastapi uvicorn docker Es necesario tener descargadas las librerias anteriores y docker en el computador. 
## como se compila y ejecuta.
### para ejecutar el servidor central: uvicorn serverc:app --reload 
### para ejecutar el pserver: python peer_server.py 
### para ejecutar el pclient: python peer_client.py download "nombre_archivo.txt" python peer_client.py upload "nombre_archivo.txt"
## detalles del desarrollo.
## detalles técnicos
## descripción y como se configura los parámetros del proyecto (ej: ip, puertos, conexión a bases de datos, variables de ambiente, parámetros, etc)
## opcional - detalles de la organización del código por carpetas o descripción de algún archivo. (ESTRUCTURA DE DIRECTORIOS Y ARCHIVOS IMPORTANTE DEL PROYECTO, comando 'tree' de linux)
## 
## opcionalmente - si quiere mostrar resultados o pantallazos 

# 4. Descripción del ambiente de EJECUCIÓN (en producción) lenguaje de programación, librerias, paquetes, etc, con sus numeros de versiones.

# IP o nombres de dominio en nube o en la máquina servidor.

## descripción y como se configura los parámetros del proyecto (ej: ip, puertos, conexión a bases de datos, variables de ambiente, parámetros, etc)

## como se lanza el servidor.

## una mini guia de como un usuario utilizaría el software o la aplicación

## opcionalmente - si quiere mostrar resultados o pantallazos 

# 5. otra información que considere relevante para esta actividad.

# referencias:
<debemos siempre reconocer los créditos de partes del código que reutilizaremos, así como referencias a youtube, o referencias bibliográficas utilizadas para desarrollar el proyecto o la actividad>
## sitio1-url 
## sitio2-url
## url de donde tomo info para desarrollar este proyecto
