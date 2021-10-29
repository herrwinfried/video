# OpenSUSE Tumbleweed Codecs Yükleme

```
sudo zypper --gpg-auto-import-keys addrepo -cfp 90 'https://ftp.gwdg.de/pub/linux/misc/packman/suse/openSUSE_Tumbleweed/' packman && sudo zypper --gpg-auto-import-keys refresh && sudo zypper --gpg-auto-import-keys dist-upgrade --from packman --allow-vendor-change && sudo zypper --gpg-auto-import-keys install -y --from packman ffmpeg gstreamer-plugins-{good,bad,ugly,libav} libavcodec-full vlc-codecs
```

https://youtu.be/ps7ktIywYwI
