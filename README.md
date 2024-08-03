# QWhiteSurGtkDecorations
Qt decoration plugin implementing WhiteSurGTK-like client-side decorations.

This project is modified based on the [QAdwaitaDecorations](https://github.com/FedoraQt/QAdwaitaDecorations) project.  

Some of the icon resources used in this project come from [WhiteSur-gtk-theme](https://github.com/vinceliuice/WhiteSur-gtk-theme.git).

## How to compile
This library uses private Qt headers and will likely not be forward nor
backward compatible. This library will have to be recompiled with every
Qt update. While it can be build using Qt 5, it is recommended to get
backported changes from Qt 6. You can get these [here](https://src.fedoraproject.org/rpms/qt5-qtwayland/blob/rawhide/f/qtwayland-decoration-support-backports-from-qt6.patch).

Build instructions:

```
mkdir build
cd build
cmake [OPTIONS] [-DUSE_QT6=true] [-HAS_QT6_SUPPORT] ..
make && make install
```

## For Archlinux users
Archlinux users can install qwhitesurgtkdecorations with aur:
```shell
yay -S qwhitesurgtkdecorations-qt5 qwhitesurgtkdecorations-qt6
```

## Usage
It can be used by setting the QT_WAYLAND_DECORATION environment variable:

```
export QT_WAYLAND_DECORATION=whitesur-gtk
```

## License
The code is under [LGPL 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html) with the "or any later version" clause.

