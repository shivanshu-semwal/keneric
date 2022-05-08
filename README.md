# keneric

The Keneric KDE (KF5) thumbnailer is a generic thumbnailer. 
It is intended to be used when there is no dedicated KDE thumbnailer 
and there is a fast and simple way to get the thumbnail image (oneliner).

## Where I found it?

- [https://forum.kde.org/viewtopic.php?f=224&t=156241#](https://forum.kde.org/viewtopic.php?f=224&t=156241#)
- [https://forum.kde.org/viewtopic.php?f=309&t=173601](https://forum.kde.org/viewtopic.php?f=309&t=173601)

## How to install

- install dependencies

```
cmake
extra-cmake-modules
kio (kio-dev / libkf5kio-dev)
```

- run following command

```sh
mkdir builddir
make
sudo make install
```
