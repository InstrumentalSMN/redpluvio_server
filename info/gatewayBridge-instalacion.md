# lInstalación en Raspberry Pi OS

[Raspberry Pi OS] se siguió este instructivo de la página de
ChirpStack

- Se agrega el repositorio:

´´´sh
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 1CE2AFD36DBCCA00

sudo echo "deb https://artifacts.chirpstack.io/packages/3.x/deb stable main" | sudo tee /etc/apt/sources.list.d/chirpstack.list
sudo apt update
´´´
- Se instala el programa:

´´´sh
sudo apt install chirpstack-gateway-bridge
´´´

- Una vez instalado nos arroja los siguientes datos de configuración:

---------------------------------------------------------------------------------
The configuration file is located at:
 /etc/chirpstack-gateway-bridge/chirpstack-gateway-bridge.toml

Some helpful commands for chirpstack-gateway-bridge:

Start:
 $ sudo systemctl start chirpstack-gateway-bridge

Restart:
 $ sudo systemctl restart chirpstack-gateway-bridge

Stop:
 $ sudo systemctl stop chirpstack-gateway-bridge

Display logs:
 $ sudo journalctl -f -n 100 -u chirpstack-gateway-bridge
---------------------------------------------------------------------------------

- Luego se instaló el lora\_gateway y packet\_forwarder siguiendo las instrucciones
del link:
<url>: <https://forum.chirpstack.io/t/compiling-packet-forwarder-on-rapsberry-pi/829/8>
otra guía:
<url>: <http://pdacontrolen.com/install-drivers-and-udp-packet-forwarder-raspberry-pi-with-gateway-rak833-version-usb-spi-lorawan-5/>












[Raspberry Pi OS]: <https://www.chirpstack.io/gateway-bridge/gateway/raspberrypi/>
