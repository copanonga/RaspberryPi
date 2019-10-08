# Snippets Raspberry Pi

Snippets para Raspberry Pi

## Índice de contenidos

- [Instalar TL-WN725N](#Instalar-TL-WN725N)
- [Actualizar Raspbian](#Actualizar-Raspbian)
- [Instalación inicial Raspberry Pi](#Instalación-inicial-Raspberry-Pi)
- [Copiar Raspbian en tarjeta SD](#Copiar-Raspbian-en-tarjeta-SD)

## Instalar TL-WN725N

Comprobamos la versión de Linux que tenemos

```
uname -a
```

Descargamos el driver en función del kernel y del modelo de Raspberry e instalamos

```
wget https://dl.dropboxusercontent.com/u/80256631/8188eu-v7-2015yyzz.tar.gz
tar xzf 8188eu-v7-2015yyzz.tar.gz
./install.sh
```

- [Fuente](https://www.raspberrypi.org/forums/viewtopic.php?f=28&t=62371&sid=9c28d58b85d7b359237267349221bdfa)

## Actualizar Raspbian

```
sudo apt-get update
sudo apt-get dist-upgrade
```

## Instalación inicial Raspberry Pi

```
sudo raspi-config
sudo apt-get update
sudo apt-get upgrade
sudo rpi-update
```

## Copiar Raspbian en tarjeta SD

Descargamos la imagen de la web oficial: [Raspbian](https://www.raspberrypi.org/downloads/)

Pasos para Mac

Obtener donde está la tarjeta SD en el Mac

```
diskutil list
```

Por ejemplo: disk4

Desmontar la tarjeta

```
diskutil unmountDisk /dev/disk4
```

Grabar la imagen

```
sudo dd bs=1m if=2015-05-05-raspbian-wheezy.img of=/dev/disk4
```

Más información en [Raspbian](https://www.raspberrypi.org/documentation/installation/installing-images/mac.md).
