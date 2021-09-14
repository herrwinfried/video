# Windows 11 WSL2/WSLg openSUSE Tumbleweed yükleme

**WSL2 İçin gerekli adımları yapmış varsayınalarak hazırlandı bu video bilginize**

## İndirme Sayfaları
- [OpenSUSE Tumbleweed İndirme Sayfası](https://download.opensuse.org/tumbleweed/appliances/) 

- [OpenSUSE Sertifikası için indirmeniz gereken sayfa](https://build.opensuse.org/package/view_file/openSUSE:Factory/shim/openSUSE-UEFI-CA-Certificate.crt?expand=1) || [Direkt sertifika Dosyasını indir](https://github.com/herrwinfried/video/releases/download/sertifika/openSUSE-UEFI-CA-Certificate.crt)

- [Direkt openSUSE-Tumbleweed-20210910-WSL.x86_64-21253.2.167.0-Snapshot20210910.appx indir](https://download.opensuse.org/tumbleweed/appliances/openSUSE-Tumbleweed-20210910-WSL.x86_64-21253.2.167.0-Snapshot20210910.appx) || [Direkt sertifika Dosyasını indir](https://github.com/herrwinfried/video/releases/download/sertifika/openSUSE-UEFI-CA-Certificate.crt)

**UYARI: WSLg Sadece Windows 11 de çalışıyor şuanlık windows 10 ilerliyen zaman belki gelebilir.**

## 3 Parti Depoyu etkinleştirip öncelikli tanımlamak (packman depo)
```bash
sudo zypper addrepo -cfp 90 'https://ftp.gwdg.de/pub/linux/misc/packman/suse/openSUSE_Tumbleweed/' packman
sudo zypper refresh
sudo zypper dist-upgrade --from packman --allow-vendor-change
```
# WSLg için yüklemeniz gereken paketler
```bash
sudo zypper dup -y
sudo zypper in -y noto-sans-fonts gsettings-desktop-schemas xorg-x11-libs xorg-x11-server humanity-icon-theme
```

### Youtube Videosu:
https://youtu.be/vD2ipbnuJEk
