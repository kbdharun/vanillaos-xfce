# Vanilla OS XFCE Image

Containerfile for building a Vanilla OS Desktop image fox XFCE.

This image is based on top of [`vanillaos/desktop`](https://github.com/Vanilla-OS/desktop-image/pkgs/container/desktop) and offers the default
Vanilla OS Desktop experience with GNOME.

## Build

```bash
sh prepare.sh
podman image build -t kbdharun/vanilla-xfce .
```

## Use this custom image

- Edit `/etc/abroot/abroot.json` with `host-shell pkexec nano /etc/abroot/abroot.json`.
- Change the "name" entry from something like `vanilla-os/desktop` to `kbdharun/vanilla-xfce`.
- Run "abroot upgrade" to switch to your custom image.
