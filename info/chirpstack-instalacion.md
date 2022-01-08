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
> Si tenías corriendo mosquitto (broker)
> desactivalo antes con:
```sh
sudo systemctl stop mosquitto
```

- para comprobar que esté corriendo acceder desde:
<http://localhost:8080/>
- más documentación en [brocaar/chirpstack-docker]



[Install Docker Engine on Ubuntu]: <https://docs.docker.com/engine/install/ubuntu/>
[Install Docker Compose]: <https://docs.docker.com/compose/install/#install-compose>
[Instalación chirpStack]: <https://www.chirpstack.io/project/guides/docker-compose/>
[brocaar/chirpstack-docker]: <https://github.com/brocaar/chirpstack-docker>
