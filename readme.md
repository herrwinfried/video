# OpenSUSE Tumbleweed Snap yükleme

```
sudo zypper --gpg-auto-import-keys addrepo --refresh https://download.opensuse.org/repositories/system:/snappy/openSUSE_Tumbleweed snappy && sudo zypper --gpg-auto-import-keys refresh && sudo zypper --gpg-auto-import-keys dup -y --from snappy && sudo zypper --gpg-auto-import-keys install snapd && sudo systemctl enable snapd && sudo systemctl start snapd && sudo systemctl enable snapd.apparmor && sudo systemctl start snapd.apparmor
```

https://youtu.be/DEUzNYNaKI4
