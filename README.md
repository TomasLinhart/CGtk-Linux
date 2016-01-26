# CGtk

CGtk is a Swift package that allows to use Gtk+ with Swift 2.2 and higher on Mac OS X. It requires Gtk+ to be installed through [homebrew](http://brew.sh/).

```bash
brew install gtk+3
```

All packages using CGtk must include header paths through extra parameters when they are built.

```bash
swift build -Xcc -I/usr/local/include/cairo -Xcc -I/usr/local/include/gtk-3.0 -Xcc -I/usr/local/include/glib-2.0/ -Xcc -I/usr/local/include/pango-1.0 -Xcc -I/usr/local/include/gdk-pixbuf-2.0 -Xcc -I/usr/local/include/atk-1.0 -Xcc -I/usr/local/lib/glib-2.0/include
```
