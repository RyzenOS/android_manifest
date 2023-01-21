
![banner](https://raw.githubusercontent.com/kutemeikito/Ryzen-Script/master/RyzenOS.jpg)
# RyzenOS

## Getting Started ## 
---------------
To get started with the RyzenOS sources, you'll need to get
familiar with [Git and Repo](https://source.android.com/setup/build/downloading).

### Requirements
- Around 500GB disk space.
- Around 16GB RAM running Linux.

To initialize your local repository, use command:

```bash
repo init -u https://github.com/RyzenOS/android_manifest.git -b tiramisu
```

## Then sync up: ##

```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build our source ###

```bash
. build/envsetup.sh
lunch ryzen_$devicecodename-userdebug
make ryzen -j$(nproc --all) | tee log.txt
```

-----------------------------------------------------------------------------
Credits:
=======
 * [**CAF**](https://source.codeaurora.org)
 * [**AOSP**](https://android.googlesource.com)
 * [**ProtonPlus**](https://github.com/protonplus-org)
 * [**LineageOS**](https://github.com/LineageOS)
 * [**ArrowOS**](https://github.com/ArrowOS)
 * [**Xdroid OSS**](https://github.com/xdroid-oss)
 * [**AncientOS**](https://github.com/ancient-lab)
 * [**PixelExperience**](https://github.com/PixelExperience)
 * [**PixelOS**](https://github.com/PixelOS-AOSP)
 * [**ProjectBlaze**](https://github.com/ProjectBlaze)
-----------------------------------------------------------------------------
