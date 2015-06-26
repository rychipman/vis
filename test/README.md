Unit tests for the low level routines used by vis
-------------------------------------------------

The testing infrastruce makes use of the tap module from the
[C Code Archive](http://ccodearchive.net). A default configuration
file is provided, but can also be (re)generated as follows:

    $ cc ccan-configurator.c
    $ ./a.out > config.h

To run the actual tests, execute `make`.

    $ make
