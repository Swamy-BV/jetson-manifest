# Axiom

Embedded AI and robotics on NVIDIA Jetson, built with Yocto.

Source manifest for **JetPack 7.2.1 / Jetson Linux R39.2.1**, using Wrynose
with ROS 2 and SWUpdate layers.

```sh
mkdir jetson
cd jetson
repo init -u https://github.com/Swamy-BV/jetson-manifest.git -b develop
repo sync
source axiom-setup.sh -b build
bitbake axiom-update
```

Sources: `sources/`. Build directory: `build/`.
Image configuration and storage layout: [meta-axiom](https://github.com/Swamy-BV/meta-axiom).
