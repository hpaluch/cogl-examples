# Port of old Cogl Examples

Here is an attempt to port Archived cogl-examples
from: https://gitlab.gnome.org/Archive/cogl

> What is Cogl? It is OpenGL wrapper used by gnome-shell, gThumb viewer and other projects.
>
> Quoting https://gitlab.gnome.org/Archive/cogl/-/blob/cogl-1.22/README.in?ref_type=heads
> > Cogl is a small open source library for using 3D graphics hardware for
> > rendering. The API departs from the flat state machine style of OpenGL and is
> > designed to make it easy to write orthogonal components that can render without
> > stepping on each others toes.

Please note that Cogl is now included inside https://gitlab.gnome.org/GNOME/mutter.
Standalone Cogl is archived and no longer maintained.
However at least Fedora still provides standalone headers/libraries.

> [!WARNING]
> Because public Cogl is archived and no longer maintained (outside `gnome-shell` fork),
> it is likely that all external programs depending on Cogl will stop working someday
> in future.
>
> You can read some information on ceased Clutter project on https://blogs.gnome.org/clutter/
> (Clutter is GUI library on top of Cogl) and on https://gitlab.gnome.org/Archive/clutter/-/tree/master
>

Requirements on Fedora 41:
```shell
sudo dnf group install 'c-development'
sudo dnf install cogl-devel
```

Tested devel package (it actually includes experimental version 2.0):
```shell
$ rpm -q cogl-devel

cogl-devel-1.22.8-11.fc41.x86_64
```

# Building

Just invoke make:
```shell
( cd cogl-hello/ && make )
```

And run with:
```shell
cogl-hello/cogl-hello
```

