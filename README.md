# Snippets Raspberry Pi

Snippets para Raspberry Pi

## Índice de contenidos

- [Instalar TL-WN725N](#Instalar-TL-WN725N)
- [Actualizar Raspbian](#Actualizar-Raspbian)

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
