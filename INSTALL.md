# Dependencies

* python2
* perl
* pandoc (to build documentation)

If you don't have pandoc, the documentation will not be built and installed.

# Installation

## From Git or source code download

You will additionally need autoconf and automake installed.

~~~
autoreconf -i
./configure
make
make install
~~~
