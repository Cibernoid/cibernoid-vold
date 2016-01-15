# cibernoid-vold
Fork of Android's volume daemon, vold.
Upstream repository: `https://android.googlesource.com/platform/system/vold/`

### Dependencies

There are no external dependencies as such. All the required libraries are part of the Android source tree itself, and will be automatically built and linked upon when building Android. However, if you want to cross-reference external code that's not part of the `vold` subproject, you must tell your IDE, cscope, or any other code browser of choice to grab code from the following directories, relative to the Android source tree root:

 - `system/core/fs_mgr/include`
 - `system/core/base/include`
 - `system/core/include`
 - `bionic/libc/include`

It is thus a prerequisite that you must have the full Android source code. Instructions for downloading and building are [here](http://source.android.com/source/requirements.html). The requirements can be summarised in that you must have a Linux or Mac OS system, with the typical development toolkit (make, git, etc.), JDK 7 and lots of free hard drive space. Also, the more free memory you have (including the swapping area), the better will the build perform. Android **loves** storage and memory.
