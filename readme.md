# Windows 11 WSL2/WSLg için Aktif etmemiz gerekenler

## Faydalandığım Linkler
[Kendi GitBook'um](https://herrwinfried.gitbook.io/tr/isletim-sistemleri/windows-11/windows-11-wsl-kurulumu-icin-gerekenler#windows-terminal-start)

## Windows Terminale Yazılacak Komutlar

```
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```

```
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```

```
DISM /Online /Enable-Feature /All /FeatureName:Microsoft-Hyper-V /norestart
```

## Windows Ayarlarda Yapılması Gerekenler 


Mavi ile işaretlenen yere gidip daha sonra yeşil ile işaretlediğim yere basın

![](https://gblobscdn.gitbook.com/assets%2F-MjDXoXaJDD0bI9oN5_-%2F-Ml-nCv0bCQEu6CMa1j6%2F-Ml-t9Wxapx-SVLIV3T3%2Fimage.png?alt=media&token=38017619-1f1c-4272-abf4-30df0f47f810)

"Diğer Microsoft ürünlerinin güncelleştirmesini al" Kapalı olarak gelceği için onu açık olarak değiştirmeniz gerekmekte. böylelikle yeni WSLg için güncelleme geldiğinde windows update aracılığı ile almış olacaksınız.

![image](https://user-images.githubusercontent.com/52379312/135824871-b0e40ef2-1f65-421b-b7c3-6966add91dd5.png)

ve bilgisayarınızı yeniden başlatın.

Windows Terminalinizi yönetici olarak başlatın ve şu komutları yazın.


```
wsl --update
```

```
wsl --shutdown
```

```
wsl --set-default-version 2
```


