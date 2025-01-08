# Device Tree Compiler and libfdt

The source tree contains the Device Tree Compiler (dtc) toolchain for
working with device tree source and binary files and also libfdt, a
utility library for reading and manipulating the binary format.

dtc and libfdt are maintained by:

* [David Gibson `<david@gibson.dropbear.id.au>`](mailto:david@gibson.dropbear.id.au)

The install depends on libfdt shared library being installed on the
host system first. Generally, using `--user` or `--prefix` is not
necessary and pip will use the default location for the Python
installation which varies if the user is root or not.

You can also install everything via make if you like, but pip is
recommended.

To install both libfdt and pylibfdt you can use:

```
$ make install [PREFIX=/path/to/install_dir]
``

More work remains to support all of libfdt, including access to numeric
values.

## Mailing lists

* The [devicetree-compiler](mailto:devicetree-compiler@vger.kernel.org)
  list is for discussion about dtc and libfdt implementation.
* Core device tree bindings are discussed on the
  [devicetree-spec](mailto:devicetree-spec@vger.kernel.org) list.

