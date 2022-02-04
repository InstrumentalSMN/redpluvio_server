# Semtech Packet Forwarder

#### global\_conf.json para AU915 en TTN
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


# SSH

#### Mantener la sesión ssh activa
<https://www.howtogeek.com/howto/linux/keep-your-linux-ssh-session-from-disconnecting/>

#### copiar un archivo local a un servidor/pc remota: [Fuente]:<https://geekytheory.com/copiar-archivos-a-traves-de-ssh-con-scp/>.
```bash
$ scp archivo.txt usuario@dominio.com:/home/usuario
```

# VIM

#### Como comentar multiples lineas: [Fuente](https://muylinux.xyz/como-comentar-varias-lineas-al-mismo-tiempo-en-el-editor-de-vim/#:~:text=Para%20hacer%20esto%2C%20vaya%20a,otras%20l%C3%ADneas%20una%20por%20una.>)
```vim
:1,4s/^/#  "Este comando comenta las líneas 1 a 4 (agrega # al ppio)
```

#### Aprender Vim en español:
<https://victorhckinthefreeworld.com/aprender-vim/>
