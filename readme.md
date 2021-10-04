# Fedora 35
## Faydalandığım Kaynaklar

https://herrwinfried.gitbook.io/tr/wslg/fedora/fedora-35-wsl2-wslg-yuekleme#gerekli-paketleri-yueklemek-ve-nano-yuekleme
https://herrwinfried.gitbook.io/tr/wslg/fedora/fedora-35-.net-swift-lang-zsh-rpmfusion-deposu-kurma-aktif-etme-wsl2-wslg

## Yazdığım Komutlar
> Temel Paketler için
```
sudo dnf install -y https://mirrors.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm https://mirrors.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm && sudo dnf update --refresh -y && sudo dnf install -y --skip-broken passwd cracklib-dicts iputils util-linux-user git curl wget dnf-plugins-core dnf-utils sudo nano
```
> Kullanıcı Hesabı Oluşturma
```
useradd -G whell USERNAME
```
> Kullanıcı Hesabına Şifre Oluşturma
```
passwd USERNAME
```
> WSL Default Kullanıcı seçme
```
touch /etc/wsl.conf && nano /etc/wsl.conf
```
```
[user]
default=USERNAME
```

> Powershell Veya CMD dönüp yazmanız gereken
```
wsl --shutdown
```

> .Net 5
```
sudo dnf install -y dotnet-sdk-5.0
```


> Swift
```
sudo dnf install -y swift-lang
```


> ZSH ve OhMyZSH
```
sudo dnf install -y zsh git curl wget
```
```
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

https://youtu.be/UBQwxLxal88
