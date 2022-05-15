## Docker
se instaló docker para Ubuntu siguiendo la páguina:
[Install Docker Engine on Ubuntu]

## Docker Compose

Se siguieron los pasos para instalación desde archivo binario
[Install Docker Compose]

## ChirpStack

- [Instalación chirpStack] Se siguó esta página y se descargó un
ejemplo desde este repositorio:
- [brocaar/chirpstack-docker] con los comandos:

```sh
git clone https://github.com/brocaar/chirpstack-docker.git
cd chirpstack-docker
```

luego...

```sh
docker-compose up
```

> Atención!
> Si no descarga los contenedores desde docker 
> agregarlo en el siguiente archivo:
```sh
vim /etc/systemd/system/docker.service.d/
```
> agregando las lineas:
```sh
[Service]
Environment="HTTP_PROXY=http://proxy-do.smn.gov.ar:8080/"

[Service]
Environment="HTTPS_PROXY=http://proxy-do.smn.gov.ar:8080/"
```

- para comprobar que esté corriendo acceder desde:
<http://localhost:8080/>
- más documentación en [brocaar/chirpstack-docker]

> Atención!
> Si tenías corriendo mosquitto (broker)
> desactivalo antes con:
```sh
sudo systemctl stop mosquitto
```



[Install Docker Engine on Ubuntu]: <https://docs.docker.com/engine/install/ubuntu/>
[Install Docker Compose]: <https://docs.docker.com/compose/install/#install-compose>
[Instalación chirpStack]: <https://www.chirpstack.io/project/guides/docker-compose/>
[brocaar/chirpstack-docker]: <https://github.com/brocaar/chirpstack-docker>
