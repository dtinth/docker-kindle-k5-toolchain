
Dockerized Toolchain for Kindle Paperwhite
==========================================

- arm (unknown)
- linux 2.6.31.14
- glibc 2.10.1
- gcc 4.3.2


Configuration
-------------

|Configuration|Value|
|----|-----|
|Default User|toolchain|
|Home Directory|/uchi|
|crosstool-ng Directory|/uchi/crosstool|
|Kindle Toolchain Directory|/uchi/kindle-toolchain|


Build
-----

    docker build -t kindle_toolchain .


Arigatou
--------

- http://wwsean08.com/2012/05/15/how-to-build-a-custom-toolchain-using-crosstool-ng/
- http://www.mobileread.com/forums/showpost.php?p=2267232&postcount=15
- http://www.mobileread.com/forums/showpost.php?p=2266891&postcount=8


