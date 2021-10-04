# openSUSE Tumbleweed

## Yardım Aldığım Linkler
[Kendi GitBook'um](https://herrwinfried.gitbook.io/tr/wslg/opensuse/tumbleweed/opensuse-tumbleweed-.net-5-dnf-zsh-codecs-opi-packman-deposunu-yuekleme)


## Yazdığım Komutlar
> .NET 5 için

```
sudo zypper --gpg-auto-import-keys install -y libicu && sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc && wget https://packages.microsoft.com/config/opensuse/15/prod.repo && sudo mv prod.repo /etc/zypp/repos.d/microsoft-prod.repo && sudo chown root:root /etc/zypp/repos.d/microsoft-prod.repo && sudo zypper --gpg-auto-import-keys ref && sudo zypper --gpg-auto-import-keys in -y dotnet-sdk-5.0
```
> DNF için
```
sudo zypper install -y dnf rpm-repos-openSUSE
```
Swap DNF yapmak isterseniz
```
sudo dnf swap -y PackageKit-backend-zypp PackageKit-backend-dnf
```

> Packman Yükleme ve Aktif etme
```
sudo zypper addrepo -cfp 90 'https://ftp.gwdg.de/pub/linux/misc/packman/suse/openSUSE_Tumbleweed/' packman && sudo zypper --gpg-auto-import-keys refresh && sudo zypper --gpg-auto-import-keys dist-upgrade --from packman --allow-vendor-change
```
> Codecs Yükleme
*Video WSL2 için gerek yok dedim ama Video oynatıcı kullancaksanız var.*
```
sudo zypper install --from packman ffmpeg gstreamer-plugins-{good,bad,ugly,libav} libavcodec-full vlc-codecs
```

> opi Yükleme
```
sudo zypper in -y opi
```

> zsh ve ohmyzsh Yükleme
```
sudo zypper in -y zsh git curl wget && sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

https://youtu.be/-7E6-_RmSog
