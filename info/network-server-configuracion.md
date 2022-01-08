# Configuración de los parámetros regionales

Cuando inicia el servidor de red (chirpstack-network-server) se cargan
las configuraciones desde el archivo "chirpstack-network-server.toml"
ubicado en  /etc/chirpstack-network-server/ dentro del contenedor.
Este archivo se copia del archivo de configuración guardado localmente
en chirpstack-docker/configuration/chirpstack-network-server/chirpstack-network-server.toml. 
- Lo descripto se  llama "persistencia de datos" (creo :) ), y se logra agregando la siguiente etiqueta dentro del archivo docker-compose.yml:

```yaml
volumes:
      - ./configuration/chirpstack-network-server:/etc/chirpstack-network-server
```
- Se cambió la linea 17 por:
```bash
name="AU915"
```

> Written with [StackEdit](https://stackedit.io/).
