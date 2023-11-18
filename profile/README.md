Project of [7Ji](https://github.com/7Ji) that combines CoreELEC and EmuELEC into one bootable media, so you can enjoy the beauty of both worlds.

Images and sources of them are hosted under the [HybridELEC](https://github.com/HybridELEC/HybridELEC) repo, there're three branches:
- `hyrbid-1.0` is the branch where it all started, it's only for Mibox3 (MDZ-16-AA), with modified CE 9.2.8 and EE v4.3, burnt onto eMMC
  - CE is the main and default distro and could not be modified
- `hybrid-ng` is a generic branch, with modified CE-ng 20 and EE-ng 4.5, burnt onto SD/USB drive
  - CE is the main and default distro and could be modified
- `android-burning` is the special branch for a few devices I own, with unmodified Android, unmodified CE and unmodified EE, burnt onto eMMC.
  - This is the only branch that I could not provide the source code, as this is done by some dirty handwork on the image directly, releasing the decompiled Android source is illegal.
  - However, I can promise the CE and EE kernel and system images are not touched at all in these images, and you can verify that by `sha256sum` them after booting.
  - Android is the default booting target, to switch to CE/EE/External, you would also need the rebooter under the [HybridELEC_Rebooter](https://github.com/HybridELEC/HybridELEC_Rebooter) repo
