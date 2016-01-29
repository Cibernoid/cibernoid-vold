# cibernoid-vold
Fork of Android's volume daemon, vold.
Upstream repository: `https://android.googlesource.com/platform/system/vold/`

### Release information

This project is an Android vold fork. It was forked from the following release cut:

 - Build: MMB29T
 - Branch: android-6.0.1_r10
 - Version: Marshmallow
 - Supported devices: Nexus Player

### Dependencies

There are no external dependencies as such. All the required libraries are part of the Android source tree itself, and will be automatically built and linked against when building Android. The header files used by `vold` are located in the following directories, relative to the Android source tree root. The actual code is written in `.c` files one level above. Should you want to cross-reference `vold` code, you should tell your IDE, cscope, or any other code browser of choice to grab code from there.

 - `system/core/fs_mgr/include`
 - `system/core/base/include`
 - `system/core/include`
 - `bionic/libc/include`

It is thus a prerequisite that you must have the full Android source code to compile `vold`. Instructions for downloading and building are [here](http://source.android.com/source/requirements.html). The requirements can be summarised in that you must have a Linux or Mac OSX system, with the typical development toolkit (make, git, etc.), JDK 7 and lots of free hard drive space. Also, the more free memory you have (including the swapping area), the better will the build perform. The Android build system **loves** memory.
