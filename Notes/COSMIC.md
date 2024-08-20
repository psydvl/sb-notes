#hacking #openSUSE #COSMIC #Desktop

# Epoch
https://github.com/pop-os/cosmic-epoch
[README:permalink](https://github.com/pop-os/cosmic-epoch/blob/8ddb4bbe6aa5347e5326cc146dea738111a30c9b/README.md)

## Install
```shell
zypper se --provides X
sudo zypper in just rust seatd-devel libxkbcommon-devel libinput-devel

# Chosen
just
rust cargo llvm-devel
# libwayland
# mesa
seatd-devel
libxkbcommon-devel
libinput-devel
# udev
dbus

# optionally (though the build-system might currently require these libraries):

# libsystem
## libpulse - openSUSE expect pipewire, trying without, maybe already installed stuff will be used
pop-launcher - trying without
# libexpat1
# libfontconfig
# libfreetype
lld
# cargo - came with rust
# libgbm-dev
# libclang-dev
# libpipewire-0.3-dev

```