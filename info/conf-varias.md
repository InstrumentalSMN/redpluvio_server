## Mantener la sesión ssh activa
<https://www.howtogeek.com/howto/linux/keep-your-linux-ssh-session-from-disconnecting/>

# Semtech Packet Forwarder

## global\_conf.json para AU915 en TTN

<https://github.com/TheThingsNetwork/gateway-conf/blob/master/AU-global_conf.json>

# Network Server / Aplication Server 

## Comandos útiles

- Para identificar el "CONTAINER ID" que luego se utiliza para ingresar a la shell del contenedor:
```bash 
sudo docker ps
```
- Para ingresar a la shell del contenedor:
```bash
sudo docker exec -i -t <CONTAINER ID> /bin/sh
```
- Para ver logs de un contenedor:
```bash
sudo docker logs <CONTAINER ID> -t -n 20
```
- Para ver logs de todos los contenedores:
Para que funcione tiene que ubicarse en la carpeta contenedora del archivo
docker-compose.yml
```bash
sudo docker-compose logs -f
```
