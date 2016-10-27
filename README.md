cod-deb-packaging
=================

Debian packaging of ``cod-tools`` software. ``cod-tools`` can be obtained
from svn://www.crystallography.net/cod-tools or GIT repository at
https://github.com/sauliusg/cod-tools.

To build any of the packages, run ``make unsigned`` inside the package
subdirectories.

The dependency tree:
```
pycodcif
  |- codcif
  |    |- libgetoptions0
  |    |    \- libcexceptions0
  |    \- libcexceptions0
  |- libgetoptions0
  |    \- libcexceptions0
  \- libcexceptions0
```
