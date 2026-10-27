# Axiom

Embedded AI and robotics on NVIDIA Jetson, built with Yocto.

Source manifest for **JetPack 7.2.1 / Jetson Linux R39.2.1**, using Wrynose
with ROS 2 and SWUpdate layers.

## Checkout

```sh
mkdir jetson
cd jetson
repo init -u https://github.com/Swamy-BV/jetson-manifest.git -b develop
repo sync
source axiom-setup.sh -b build
bitbake axiom-image
```

Sources are checked out under `sources/`. Upstream revisions are pinned from the latest
Wrynose branch heads as of 2026-10-26; BitBake uses the corresponding `2.18`
branch. `meta-axiom` follows `develop`.
