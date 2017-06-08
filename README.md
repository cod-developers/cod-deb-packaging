cod-deb-packaging
=================

Debian packaging of ``cod-tools`` software. ``cod-tools`` can be 
obtained from svn://www.crystallography.net/cod-tools or GIT 
repository at https://github.com/sauliusg/cod-tools.

Installation
------------

To build all of the packages, run ``make all``. In total, nine
packages are build out of ``cod-tools`` source.

Dependency tree
---------------

```
cod-tools
  |- libcod-cif-parser-bison-perl
  |   |- codcif (build)
  |   |    |- libgetoptions0 (build)
  |   |    |    \- libcexceptions0 (build)
  |   |    \- libcexceptions0 (build)
  |   |- libcexceptions0 (build)
  |   |- libcod-precision-perl
  |   \- libcod-usermessage-perl
  |- libcod-cif-parser-yapp-perl
  |   |- libcod-precision-perl
  |   \- libcod-usermessage-perl
  |- libcod-precision-perl
  \- libcod-usermessage-perl

python-pycodcif
  |- codcif (build)
  |    |- libgetoptions0 (build)
  |    |    \- libcexceptions0 (build)
  |    \- libcexceptions0 (build)
  |- libgetoptions0 (build)
  |    \- libcexceptions0 (build)
  \- libcexceptions0 (build)
```
