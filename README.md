# supergfxctl-plasmoid

KDE Plasma plasmoid for [supergfxctl](https://gitlab.com/asus-linux/supergfxctl)  
Built as a C++/QML Plasmoid

## Features

- [x] Graphics mode switching
- [x] dGPU power indication
- [x] Dynamic plasmoid logo, tooltip
- [x] Filter available switches
- [x] Display dbus error message
- [x] Alert 180 second timeout on logout
- [x] Revert change (to compute, integrated, vfio)
- [ ] Revert change (to hybrid, nvidia)

## Screenshots

<img src="https://gitlab.com/jhyub/supergfxctl-plasmoid/-/raw/master/screenshots/filter.png" alt="filter.png" width="300">

Default menu, on hybrid mode

<img src="https://gitlab.com/jhyub/supergfxctl-plasmoid/-/raw/master/screenshots/switching.png" alt="switching.png" width="300">

While switching

<img src="https://gitlab.com/jhyub/supergfxctl-plasmoid/-/raw/master/screenshots/error.png" alt="error.png" width="300">

Display dbus errors

<img src="https://gitlab.com/jhyub/supergfxctl-plasmoid/-/raw/master/screenshots/revert.png" alt="revert.png" width="300">

Revert menu

## Installation
### Arch User Repository
[kdeplasma-applets-supergfxctl](https://aur.archlinux.org/packages/kdeplasma-applets-supergfxctl)
### Build yourself

```shell
git clone https://gitlab.com/Jhyub/supergfxctl-plasmoid
cd supergfxctl-plasmoid
git checkout [LATEST VERSION TAG HERE]
mkdir build
cd build
cmake -DCMAKE_INSTALL_PREFIX=/usr ..
make
sudo make install # or any other elevation tool
```
#### Fedora
Build dependencies are: `git` `cmake` `gcc-c++` `extra-cmake-modules` `kf5-ki18n-devel` `kf5-plasma-devel` `qt5-qtdeclarative-devel`

## Copyright Notice
Some files under ./icons/status are from or derived from [asusctl-gex](https://gitlab.com/asus-linux/asusctl-gex), which is distributed under the Mozilla Public License 2.0.
The following is an exhaustive list of files.  
```
supergfxctl-plasmoid-dgpu-active.svg
supergfxctl-plasmoid-dgpu-off.svg
supergfxctl-plasmoid-dgpu-suspended.svg
supergfxctl-plasmoid-gpu-copute.svg
supergfxctl-plasmoid-gpu-compute-active.svg
supergfxctl-plasmoid-gpu-egpu.svg
supergfxctl-plasmoid-gpu-egpu-active.svg
supergfxctl-plasmoid-gpu-hybrid.svg
supergfxctl-plasmoid-gpu-hybrid-active.svg
supergfxctl-plasmoid-gpu-integrated.svg
supergfxctl-plasmoid-gpu-integrated-active.svg
supergfxctl-plasmoid-gpu-nvidia.svg
supergfxctl-plasmoid-gpu-nvidia-active.svg
supergfxctl-plasmoid-gpu-vfio.svg
supergfxctl-plasmoid-gpu-vfio-active.svg
```
