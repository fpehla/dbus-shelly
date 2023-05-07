How to install everything required for this Mod on Venus OS

## Install Python PIP 

```
opkg update
opkg install python3-pip
```

## Install Python modules

```
pip3 install websockets
pip3 install dbus_next
```

## Copy Sources and  ext/aiovelib to Venus OS

* Install (make install) to a Temp directory
* Rsync the Temp directory to /data/dbus-shelly on Venus OS

## On Venus OS

Symlink to service directory to get service started automatically

```
ln -s /data/dbus-shelly/service /service/dbus-shelly
```
