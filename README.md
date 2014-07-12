
Dockerized Toolchain for Kindle Paperwhite
==========================================

- arm (unknown)
- linux 2.6.31.14
- eglibc 2.12
- linaro-gcc 4.7


Configuration
-------------

|Configuration|Value|
|----|-----|
|Default User|toolchain|
|Home Directory|/uchi|
|crosstool-ng Version|1.19.0|
|crosstool-ng Directory|/uchi/crosstool|
|Kindle Toolchain Directory|/uchi/kindle-toolchain|


crosstool-ng
------------

|Configuration|Value|
|-------------|-----|
|Base|arm-cortex_a8-linux-gnueabi|
|Target: Target CFLAGS|`-O2 -fomit-frame-pointer -pipe`|
|Toolchain: Tuple's vendor string|`kindle_k5`|
|OS: Target kernel version|`2.6.31.14`|
|Binary utilities: binutils|`2.22`|
|Binary utilities: Linkers to enable|`ld,gold`|
|C compiler: show linaro|yes|
|C compiler: gcc version|`linaro-4.8-2013.06-1`|
|C compiler: enable LTO|yes|
|C library|`eglibc`|
|C library: version|`2.12`|
|Debug facilities|none|

Build
-----

    docker build -t kindle_toolchain .


Arigatou
--------

- http://wwsean08.com/2012/05/15/how-to-build-a-custom-toolchain-using-crosstool-ng/
- http://www.mobileread.com/forums/showpost.php?p=2267232&postcount=15
- http://www.mobileread.com/forums/showpost.php?p=2266891&postcount=8




