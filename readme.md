# Arch

## Faydalandığım Kaynaklar
https://herrwinfried.gitbook.io/tr/wslg/arch-linux/arch-wsl2-wslg-yuekleme#ve-artik-hazir

## Yazmamız gereken komutlar

> Temel Komutlar

```
pacman -Syy && pacman-key --init && pacman-key --populate && pacman -Syu && pacman -S nano
```


> Kullanıcı Hesabı Oluşturma

```
useradd -mg users -G storage,wheel,power -s /bin/bash USERNAME
```
> Kullanıcıya Şifre Oluşturma

```
passwd USERNAME
```

> Sudoers Dosyası Düzenleme

*#%whell ALL=(ALL) ALL başındaki # kaldırın son hali böyle olmalı
%whell ALL=(ALL) ALL*
sudoers dosyasını düzenliyelim ve yukardaki bahsettiğim olayı yapalım

```
nano /etc/sudoers
```
> Powershell veya cmd yazmamız gereken komut
```
Arch.exe config --default-user USERNAME
```
https://youtu.be/inKtj70JhpI
