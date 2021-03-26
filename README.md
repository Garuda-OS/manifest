# Garuda-OS

<centre> Yet Another cherry-picked Custom ROM FUELED BY LINEAGE-OS <centre/>

<img src="https://github.com/Garuda-OS/manifest/blob/eleven/banner.jpeg?raw=true">

Credits:
=======
 * [**Cipher OS**](https://github.com/CipherOS)
 * [**RevengeOS**](https://github.com/RevengeOS)
 * [**AOSP**](https://android.googlesource.com)
 * [**LineageOS**](https://github.com/LineageOS)
 * [**DirtyUnicorns**](https://github.com/dirtyunicorns)
 * [**PixelExperience**](https://github.com/PixelExperience)
 * [**Project-Awaken**](https://github.com/Project-Awaken)
 * [**POSP**](https://github.com/PotatoProject)
 * [**Project-Streak**](https://github.com/ProjectStreak)
 * [**LineageOS**](https://github.com/LineageOS)
 * [**FusionOS**](https://github.com/Fusion-OS)
 * [**POSP**](https://github.com/POSP)
-----------------------------------------------------------------------------


Getting Started:
==============

To get started with the building process, you'll need to get familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

### Initializing & sync Repo ###

```bash
# Initialize repo
repo init -u git://github.com/Garuda-OS/manifest.git -b eleven

# Sync 
repo sync -c -q --force-sync --optimized-fetch --no-tags --no-clone-bundle --prune -j$(nproc --all)
```

### Building the ROM ###

```bash
# Set up environment 
$ . build/envsetup.sh

# Choose a target device 
$ lunch lineage_($device_codename)-userdebug

# Compile Garuda-OS

$ mka bacon -j$(nproc --all)
```
