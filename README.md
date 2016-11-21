cod-deb-packaging
=================

Debian packaging of ``cod-tools`` software. ``cod-tools`` can be obtained
from svn://www.crystallography.net/cod-tools or GIT repository at
https://github.com/sauliusg/cod-tools.

Installation
------------

To build any of the packages, run ``make unsigned`` inside the package
subdirectories. Be aware that some of the packages depend on others in
this collection. Please refer to the following dependency tree.

Dependency tree
---------------

```
pycodcif
  |- codcif
  |    |- libgetoptions0
  |    |    \- libcexceptions0
  |    \- libcexceptions0
  |- libgetoptions0
  |    \- libcexceptions0
  \- libcexceptions0

libcod-precision-perl

libcod-usermessage-perl
```
