# Setup Apache Nifi

## Chequeo inicial
Primero tenemos que asegurarnos que se está ejecutando docker en nuestros ordenadores con el comando :
```bash
docker ps
```
ejemplo:
```bash
(base) Ramon-Marquez-MBP15:BigDataUFV ramon$ docker ps
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
```
si la salida da algún tipo de error como 
```bash
(base) Ramon-Marquez-MBP15:BigDataUFV ramon$ docker ps
Cannot connect to the Docker daemon at unix:///Users/ramon/.docker/run/docker.sock. Is the docker daemon running?
```
Es porque no se ha inicializado el proceso docker.

Tenemos que tener descargado de Git la última versión del repositorio.

## Inicialización Apache Nifi

Dentro de la carpeta Apache Nifi ejecutamos en linea de comando (PowerShell para Windows y Terminal para Mac)
```bash
docker-compose up -d
```
Nos aparecerá un pull (se están descargando las imagenes si es la primera vez) y luego un **Started**, ejemplo:
```bash
base) Ramon-Marquez-MBP15:Apache Nifi ramon$ docker-compose up -d
[+] Running 1/1
 ✔ Container nifi  Started                                                 3.1s 
 ```
Luego de 5 minutos aproximadamente ver si podemos acceder a la consolo de desarrollo en : **http:localhost:8080**
Debería de aparecer algo como:
<img src="img/nifihomepage.png" width="400" height="350">

[Volver al Menú Principal](https://github.com/jr-marquez/BigData_UFV/blob/main/README.md#apache-nifi)