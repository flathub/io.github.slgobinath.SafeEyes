# io.github.slgobinath.SafeEyes

Safe Eyes is a Free and Open Source tool for Linux users to reduce and prevent repetitive strain injury (RSI).

For upstream issues:
    https://github.com/slgobinath/SafeEyes/issues

<!-- ### Non-functional plugins:

- xprintidle

`xprintidle` calls `XScreenSaverQueryExtension()` on the display specified in the DISPLAY environment variable to check if the `XScreenSaver` extension is available

If that call returns false xprintidle exits with "screen saver extension not supported".

And currently just spams `screen saver extension not supported`

https://github.com/g0hl1n/xprintidle/issues/9

- wlrctl -->

### Build yourself

```bash
# clone this repo
git clone --recursive https://github.com/flathub/io.github.slgobinath.SafeEyes && cd io.github.slgobinath.SafeEyes
# install flatpak and flatpak-builder then add flathub
sudo apt install flatpak flatpak-builder && flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo
# install flatpak runtime
flatpak install -y org.freedesktop.Sdk/x86_64/24.08
# build
flatpak-builder --user --install --force-clean build-dir io.github.slgobinath.SafeEyes.yaml
```
