# Windows 11'e [Beta] WSA Aurora Store ve Termux yükleme

## Linkler

- [ADB İndirme Yeri](https://developer.android.com/studio/releases/platform-tools)
- [Aurora Store İndirme Sayfası](https://auroraoss.com/download/)
- [Aurora Store files sayfası](https://files.auroraoss.com/AuroraStore/Stable/)


- [platform-tools-latest-windows.zip{ADB} Direkt İndir](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)
- [AuroraStore_4.0.7.apk Direkt İndir](https://files.auroraoss.com/AuroraStore/Stable/AuroraStore_4.0.7.apk)
> video izleyerek yapmanızı öneririm karışk gelebilir yöntemler.

### WSA açık olması gerekenler
 - Geliştirici Modu(Developer Mode)

### ADB için yapmamız gerekenler
"platform-tools-latest-windows.zip"  Tümüne ayıkla diyip çıkartıyoruz 

daha sonra klasörün içine girip adb uygulamasın olduğu yerde sağ tık yapıp windows terminal ile aç diyoruz

daha sonra WSA 'daki Geliştirici Modu(Developer mode) altındaki "Geliştirici Ayarları Yönetme" Basıyoruz 

ve oradanda "Kablosuz Hata Ayıklama" Tıklıyoruz Ordaki Yazan IP Adresimizi not alalım
> Örn: 192.168.1.1:5555 yazıyorsa 192.168.1.1 kısmını not alın.

Terminalimize dönüp Powershell 7 veya Windows Powershell'e
> cmd ile açarsanız `.\adb` değil `adb` yazmalısınız.

> **Örnek** `.\adb connect 192.168.1.1`
```
.\adb connect IPadres
```
> hata verirse kapatıp terminali yeniden deneyin already veya başarılı yazısı görmeniz gerekiyor. bağlı cihazları kontrol etmek için `.\adb devices`

## APK Yükleme && Aurora Store yükleme
> örnek: Bende Masaüstümde win klasörümün içinde yüklü aurora store Hesabımın adıda winfried ` .\adb install "C:\Users\winfried\desktop\win\AuroraStore_4.0.7.apk` şeklinde yolu izlemem gerekir.
```
.\adb install "DosyanınTamYolu\Dosyaadi.uzantısı
```

### Termux kurulumu

Aurora store kurduktan sonra içinden termux indirip yükliyebilirsiniz.

> Termux ta pkg update yaparken yasak diye forbidden diye yani hata alırsanız. yazmanız gereken komut termuxa
```
rm ../usr/etc/apt/sources.list.d/*
```

### Termux neofetch yükleme

```
pkg install neofetch
```
https://youtu.be/_mpvONtMv8k
