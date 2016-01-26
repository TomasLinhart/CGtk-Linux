# CGtk

CGtk is a Swift package that allows to use Gtk+ with Swift 2.2 and higher on Linux (Ubuntu). It requires Gtk+ and Clang to be installed.

```bash
sudo apt-get install libgtk-3-dev clang
```

All packages using CGtk must include header paths through extra parameters when they are built.

```bash
swift build -Xcc -I/usr/include/cairo -Xcc -I/usr/include/gtk-3.0 -Xcc -I/usr/include/glib-2.0 -Xcc -I/usr/include/pango-1.0 -Xcc -I/usr/include/gdk-pixbuf-2.0 -Xcc -I/usr/include/atk-1.0 -Xcc -I/usr/lib/x86_64-linux-gnu/glib-2.0/include
```

It is currently used by [SwiftGtk](https://github.com/TomasLinhart/SwiftGtk).
