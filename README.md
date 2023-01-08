# gnome-screenshot-noflash

This is a mirror of https://gitlab.gnome.org/GNOME/gnome-screenshot with
**flash** feature permanently turned off.

`bin/build` for build and `bin/install` for installation.

## Building in Ubuntu 22.04

```shell
docker run --rm -i ubuntu:22.04 << 'EOF'
cd
apt update
DEBIAN_FRONTEND=noninteractive apt install -y git meson build-essential gettext libglib2.0-dev libgtk-3-dev libhandy-1-dev

git clone https://github.com/vbarbarosh/gnome-screenshot-noflash
cd gnome-screenshot-noflash
bin/build
EOF
```

## Building in Ubuntu 22.10

```shell
docker run --rm -i ubuntu:22.10 << 'EOF'
cd
apt update
DEBIAN_FRONTEND=noninteractive apt install -y git meson build-essential gettext libglib2.0-dev libgtk-3-dev libhandy-1-dev

git clone https://github.com/vbarbarosh/gnome-screenshot-noflash
cd gnome-screenshot-noflash
bin/build
EOF
```

GNOME Screenshot
================

GNOME Screenshot is a small utility that takes a screenshot of the whole
desktop; the currently focused window; or an area of the screen.

### Dependencies

 - GLib 2.36
 - GTK+ 3.12
 - X11
