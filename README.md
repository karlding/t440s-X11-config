# Lenovo T440s X11 configuration
My X11 configuration settings for the Synaptics Trackpad on the Lenovo Thinkpad T440s. I was having trouble getting Ubuntu 16.04 LTS to detect my trackpad as a trackpad (and not a mouse), even though ``xinput`` could recognize the device.

With this configuration, the Trackpad shows up under Mouse & Touchpad settings, and we can configure things like Natural Scrolling for just the Trackpad. In addition, things like tap to click and the tap and drag gestures also work.

## Setup
Basically, symlink (or copy) the ``xorg.conf`` and ``xorg.conf.d`` directories to ``/etc/X11``.

```bash
cd ~
git clone https://github.com/karlding/t440s-X11-config.git
ln -sf ~/t440s-X11-config/xorg.conf /etc/X11/xorg.conf
ln -sf ~/t440s-X11-config/xorg.conf.d /etc/X11/xorg.conf.d
```
