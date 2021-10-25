# Windows 11'e [Beta] Windows Subsystem for Android yükleme

> "Sanal Makine Platform" Özelliği Aktif Olması Gereklidir.Windows Terminalizi Yönetici Olarak Çalıştırın.
> 
> ```
> dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
> ```

## Linkler
- [https://store.rg-adguard.net/](https://store.rg-adguard.net/)

- [https://www.microsoft.com/store/productId/9P3395VX91NR9](https://www.microsoft.com/store/productId/9P3395VX91NR)

### Adguard Sayfasında yapılması gerekenler

1. İlk Button URL olarak seçtiğinizden emin olun

2. doldurulması gereken forma https://www.microsoft.com/store/productId/9P3395VX91NR yazdığınızdan emin olun.

3. RP yerine Slow seçili olduğundan emin olun

.msixbundle dosyasını bulun `örnek: MicrosoftCorporationII.WindowsSubsystemForAndroid_1.7.32815.0_neutral_~_8wekyb3d8bbwe.msixbundle`

yaklaşık 1.20+ GB olduğundan emin olun.


### Dosyayı İndirdikten sonra yapılması gerekenler

Windows Terminali Yönetici Olarak çalıştırın ve Powershell seçiniz.

> __**Dikkat!** Powershell 7 kullanıyorsanız öncesinde__
```
Import-Module -Name Appx -UseWIndowsPowershell 
```
> komutunu yazmalısınız. Eğer Powershell 7 kullanmıyorsanız zaten pencere adıda değiştirmediyseniz Windows Powershell olarak gözükcektir Windows Powershell ise gerek yoktur.
ardından indirdiğiniz yere gidin.


> indirilenler klasörüne yüklediyseniz tahminen `cd .\Downloads\`
```
cd .\Desktop\
```

Daha Sonra dosyamızı yüklememiz gerekiyor
> Örnek: `Add-AppxPackage .\DOSYAADI.Msixbundle`
```
Add-AppxPackage .\MicrosoftCorporationII.WindowsSubsystemForAndroid_1.7.32815.0_neutral___8wekyb3d8bbwe.Msixbundle
```

https://youtu.be/1YzlmSRS8O0
