# Windows 11 WSL2/WSLg Fedora 34 yükleme

**WSL2 İçin gerekli adımları yapmış varsayınalarak hazırlandı bu video bilginize**

## İndirme Sayfaları

- [Fedora Container Sayfası](https://koji.fedoraproject.org/koji/packageinfo?packageID=26387)

- [Direkt Fedora-Container-Base-34-20210914.0.x86_64.tar.xz indirme](Fedora-Container-Base-34-20210914.0.x86_64.tar.xz)

**UYARI: WSLg Sadece Windows 11 de çalışıyor şuanlık windows 10 ilerliyen zaman belki gelebilir.**
# Sırasıyla Komutlar

- ## 1- PowerShell Komutları

> `mkdir DağıtımınDepolancağıKonum`

> `wsl --import Dağıtımİsmi DağıtımınDepolancağıKonum DağıtımınİçindekiLayer.tarDosyasınKonumu`

> `wsl -d Dağıtımİsmi` 

```powershell
mkdir $HOME\wsl2\fedora
wsl --import fedora $HOME\wsl2\fedora layer.tar
wsl -d fedora
```

- ## 2- Bash Komutları
> `grau` diye adlandırdığım kısımlara kendi kullanıcı adınızı yazıcaksınız.
```bash
sudo dnf install -y passwd cracklib-dicts iputils util-linux-user
useradd -G whell grau
passwd grau
logout
```

- ## 3- PowerShell komutları
> `grau` diye adlandırdığım kısımlara kendi kullanıcı adınızı yazıcaksınız.

```bash
wsl -d fedora -u grau
```


## 3 Parti Depoyu aktifleştirmek (rpmfusion depo)
```bash
sudo dnf install -y https://mirrors.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm https://mirrors.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm && sudo dnf update
```

# WSLg için yüklemeniz gereken paketler
*Normal Şartlarda Gerek yok*

### Youtube Videosu:
https://youtu.be/_8uhiseVfHA
