# OpenSUSE Tumbleweed Chrome Yükleme
```
sudo zypper --gpg-auto-import-keys install -y wget && wget https://dl.google.com/linux/linux_signing_key.pub && sudo rpm --import linux_signing_key.pub && wget https://dl.google.com/linux/direct/google-chrome-stable_current_x86_64.rpm -O google-chrome-stable_current_x86_64.rpm && sudo zypper --gpg-auto-import-keys ref && sudo zypper --gpg-auto-import-keys in -y ./google-chrome-stable_current_x86_64.rpm
```

https://youtu.be/oc9FOQSZClg
