# HDMI issue with Intel Arc GPU not sound after Boot on Fedora/Nobara

To Fix disable "load-module module-suspend-on-idle" under /etc/pulse/default.pa.

```
sudo sed -i 's/load-module module-suspend-on-idle/#load-module module-suspend-on-idle/' /etc/pulse/default.pa
pulseaudio -k
```
