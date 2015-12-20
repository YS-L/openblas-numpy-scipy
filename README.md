Compile and install numpy and scipy linked with OpenBLAS. This makes them fast.

Currently supports:
* Ubuntu

Build and install
-----------------
Execute the following script

```
$ setup
```
and the fast numpy stack linked with OpenBLAS will be compiled and installed.

The OpenBLAS library will be installed to ``$HOME/install``. The numpy and
scipy will be installed with the ``--user`` flags, which means that the
packages will reside in ``$HOME/.local/``.

Or manually, run the following in sequence (which is what the above ``setup``
script does):

```
$ get_sources
$ make_openblas
$ make_numpy
$ make_scipy
```
