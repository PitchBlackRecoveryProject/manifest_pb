Getting Started
======

To get started with PitchBlack Recovery, you'll need to get
familiar with [Git and Repo](https://source.android.com/source/using-repo.html).

To initialize your local repository using the minimal-manifest-twrp omni trees to build PBRP, use a command like this:
```bash
$ repo init -u git://github.com/PitchBlack-Recovery/manifest_pb.git -b PBRP
```
 For Initial Low RAM Devices or older MTK Devices:
```bash
$ repo init -u git://github.com/PitchBlack-Recovery/manifest_pb.git -b twrp-6.0
```
To initialize a shallow clone, which will save even more space, use a command like this:
```bash
$ repo init --depth=1 -u git://github.com/PitchBlack-Recovery/manifest_pb.git -b PBRP
```
For Initial Low RAM Devices:
```bash
$ repo init --depth=1 -u git://github.com/PitchBlack-Recovery/manifest_pb.git -b twrp-6.0
```
Then to sync up:
```bash
$ repo sync
```

Then to build:
```bash

     $ cd <source-dir>
     
     $ export ALLOW_MISSING_DEPENDENCIES=true
     
     $ . build/envsetup.sh
    
     $ lunch omni_<device>-eng
     
     $ mka recoveryimage
```
