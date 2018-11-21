<div align="center">
<img src ="PitchBlack-Banner.png">
</div>
<h1 align="center">
PitchBlack Recovery Project
</h1>
<h2 align="center">
An Open Source custom recovery for android
</h2>

<div align="center">
<a href="#">
  <img src="https://img.shields.io/badge/platform-android-blue.svg?style=flat-square"
    alt="platform" />
</a>

<a href="#">
  <img src="https://img.shields.io/badge/build-stable-brightgreen.svg?style=flat-square"
    alt="build" />
</a>

<a href="#">
  <img src="https://img.shields.io/badge/version-2.9.0-green.svg?style=flat-square"
    alt="version">
</a>
<a href="#">
  <img src="https://img.shields.io/badge/base-twrp 3.2.3-orange.svg?style=flat-square"
    alt="base">
</a>

</a>
<a href="https://github.com/PitchBlackRecoveryProject/android_bootable_recovery/blob/PBRP/LICENSE">
  <img src="https://img.shields.io/badge/license-apache%202.0-3F51B5.svg?style=flat-square"
    alt="base">
</a>

</div>

<br>
<h3 align="center">
Getting started
</h3>
<br>

To get started with PitchBlack Recovery, you'll need to get
familiar with [Git and Repo](https://source.android.com/source/using-repo.html).

To initialize your local repository using the minimal-manifest-twrp omni trees to build PBRP, use a command like this:
```bash
$ repo init -u git://github.com/PitchBlackRecoveryProject/manifest_pb.git -b PBRP
```
 For Initial Low RAM Devices or older MTK Devices:
```bash
$ repo init -u git://github.com/PitchBlackRecoveryProject/manifest_pb.git -b twrp-6.0
```
To initialize a shallow clone, which will save even more space, use a command like this:
```bash
$ repo init --depth=1 -u git://github.com/PitchBlackRecoveryProject/manifest_pb.git -b PBRP
```
For Initial Low RAM Devices:
```bash
$ repo init --depth=1 -u git://github.com/PitchBlackRecoveryProject/manifest_pb.git -b twrp-6.0
```
Then to sync up:
```bash
$ repo sync
```

Then to build:
```bash

     $ cd <source-dir>

     $ . build/envsetup.sh

     $ lunch omni_<device>-eng

     $ mka recoveryimage
```

If it fails to build:
```bash

     $ export LC_ALL=C
```
