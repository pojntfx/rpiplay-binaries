# RPiPlay Binaries

Weekly builds of https://github.com/FD-/RPiPlay.

![hydrun CI](https://github.com/pojntfx/rpiplay-binaries/workflows/hydrun%20CI/badge.svg)

## Installation

Binaries are built weekly and uploaded to [GitHub releases](https://github.com/pojntfx/rpiplay-binaries/releases).

On Fedora 34 (other RHEL-like distros should work too), you can install them like so:

```shell
$ sudo dnf install -y gstreamer1 # You will need to install GStreamer. The rest of the dependencies are bundled into the static binary.
$ curl -L -o /tmp/rpiplay https://github.com/pojntfx/rpiplay-binaries/releases/download/latest/rpiplay-linux.fedora.static.$(uname -m) # Stip `.static` to get a non-static binary; see https://github.com/FD-/RPiPlay#fedora-33 for bundled dependencies
$ sudo install /tmp/rpiplay /usr/local/bin
```

On Debian 10 (other Debian-like distros should work too), you can install them like so:

```shell
$ sudo apt install -y gstreamer-1.0 # You will need to install GStreamer. The rest of the dependencies are bundled into the static binary.
$ curl -L -o /tmp/rpiplay https://github.com/pojntfx/rpiplay-binaries/releases/download/latest/rpiplay-linux.debian.static.$(uname -m) # Stip `.static` to get a non-static binary; see https://github.com/FD-/RPiPlay#ubuntu-1804-or-2004 for bundled dependencies
$ sudo install /tmp/rpiplay /usr/local/bin
```

## License

RPiPlay Binaries (c) 2021 Felicitas Pojtinger and contributors

SPDX-License-Identifier: GPL-3.0
