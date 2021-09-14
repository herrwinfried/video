# Windows 11 WSL2/WSLg Arch Linux yükleme

**WSL2 İçin gerekli adımları yapmış varsayınalarak hazırlandı bu video bilginize**

## İndirme Sayfaları

- [ArchWSL Projesinin Github Sayfası](https://github.com/yuk7/ArchWSL)

- [ArchWSL-AppX_21.8.28.0_x64.appx](https://github.com/yuk7/ArchWSL/releases/download/21.8.28.0/ArchWSL-AppX_21.8.28.0_x64.appx)

- [ArchWSL-AppX_21.8.28.0_x64.cer (Sertifika)](https://github.com/yuk7/ArchWSL/releases/download/21.8.28.0/ArchWSL-AppX_21.8.28.0_x64.cer)

- [ArchWSL Relase 21.8.28.0](https://github.com/yuk7/ArchWSL/releases/tag/21.8.28.0)

**UYARI: WSLg Sadece Windows 11 de çalışıyor şuanlık windows 10 ilerliyen zaman belki gelebilir.**

# Sırasıyla Komutlar

- ## 1- Bash Komutları

> `grau` diye adlandırdığım kısımlara kendi kullanıcı adınızı yazıcaksınız.

```bash
pacman -Syy && pacman -Syu
pacman-key --init && pacman-key --populate
pacman -Syu
useradd -mg users -G storage,wheel,power -s /bin/bash grau
passwd grau
```

> sudoers dosyasından gerekli dosyaları # kaldırmalısınız.

> `%whell ALL=(ALL) ALL` adlı yazının başındaki `#` kaldırmalısınız tam uyuştundan emin olun kelimenin.

```bash
nano /etc/sudoers
```

- ## 2- PowerShell Komutları

> `grau` diye adlandırdığım kısımlara kendi kullanıcı adınızı yazıcaksınız.

```bash
Arch.exe config --default-user grau
```

# WSLg için yüklemeniz gereken paketler
*Normal Şartlarda Gerek yok*

### Youtube Videosu:
https://youtu.be/X-eC0oVhflA
