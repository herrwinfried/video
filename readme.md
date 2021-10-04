# Fedora 35 (Sadece Kurulum)
> Sadece Kurulumu Göstermektedir. Kullanıcı oluşturma dahil değildir.

## Faydalandığım Kaynaklar

[Kendi GitBook'um](https://herrwinfried.gitbook.io/tr/wslg/fedora/fedora-35-wsl2-wslg-yuekleme)

## Linkler

[Fedora Container Base Sayfası](https://koji.fedoraproject.org/koji/packageinfo?packageID=26387)

[Fedora-Container-Base-35-20211003.n.0 Sayfası](https://koji.fedoraproject.org/koji/buildinfo?buildID=1839635)

[Fedora-Container-Base-35-20211003.n.0 İndir](https://kojipkgs.fedoraproject.org//packages/Fedora-Container-Base/35/20211003.n.0/images/Fedora-Container-Base-35-20211003.n.0.x86_64.tar.xz)

## Windows Terminale Yazdığımız Komutlar

```
mkdir $HOME\wsl2\fedora
```
> ipucu `wsl --import <Dağıtımİsmi> <DepolancağıKonum> <layer.tarTamKonumu>`

```
wsl --import fedora $HOME\wsl2\fedora layer.tar
```

```
wsl -d fedora
```
https://youtu.be/CWpeEuPbzMI
