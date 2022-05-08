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

## How to use

To use the Keneric thumbnailer will need:

- Shared library file: `keneric.so`
- Desktop file for the thumbnailer. In this case: `kenricfolder.desktop`
  - Paste this in location given by `kf5-config --path services`
- Exeutable script file: `stripPicture`
  - Paste this in the location specified int the `$PATH` variable
  - Modify the script for your own use. My script generate `inode/directory` mime type
    thumbnails you can generate for other mime type too.