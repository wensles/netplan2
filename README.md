# netplan++ - A new and improved version of Netplan.io!

# Documentation

An overview of the architecture can be found at [netplan.io/design](https://netplan.io/design)

The full documentation for netplan is available in the [doc/](../main/doc/) directory.

Netplan's [documentation objectives](https://docs.google.com/document/d/1n47hwLmR6GiLJX0t5w2_uGngQ3b3jfpPN8H8knIJ9vQ) (internal)

# Build using Meson

Steps to build netplan using the [Meson](https://mesonbuild.com) build system inside the `build/` directory:

* meson setup build --prefix=/usr [-Db_coverage=true]
* meson compile -C build
* meson test -C build --verbose [TEST_NAME]
* meson install -C build --destdir ../tmproot
