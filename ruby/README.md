
Dockerfile for Cross-Compiling Ruby for Kindle Paperwhite
=========================================================


Configuration
-------------

|Ruby Source Code Directory|/uchi/ruby-2.1.2|
|Kindle Installation Path|/mnt/us/ruby-2.1.2|


Usage
-----

    docker build -t kindle_ruby .
    docker run kindle_ruby tar cvj -C /mnt/us ruby-2.1.2 > ruby-2.1.2-kindle.tar.bz2