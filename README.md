### First Download AOSP Source Code
        repo init -u https://android.googlesource.com/platform/manifest -b android-7.1.1_r55
        repo sync -j8

### Then Download these projects, replacing the AOSP source code
        rm -rf ./frameworks/native
        rm -rf ./bionic
        rm -rf ./external/kernel-headers
        git clone http://github.com/dustinmcafee/ESM_native.git			./frameworks
        git clone http://github.com/dustinmcafee/ESM_bionic.git
        git clone http://github.com/dustinmcafee/ESM_kernel-headers.git		./external
        git clone http://github.com/dustinmcafee/ESM.git			./kernel

### For more information:
        git clone http://github.com/dustinmcafee/ESM_writeup.git
