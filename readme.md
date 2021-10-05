# Windows 11 WSLg/WSL2 Ram Miktarı ve İşlemci Sayısını değiştirme

## Yazdığım komutlar
```
wsl --shutdown
```

```
notepad "$env:USERPROFILE/.wslconfig"
```
> İşlemci Sayısı Ve ram Miktarını değiştirme
```
[wsl2]
memory=12GB   # WSL 2'deki VM belleğini 12 GB'a kadar sınırlar
processors=4 # WSL 2 VM'nin iki sanal işlemci kullanmasını sağlar
```

https://youtu.be/mii0L6g8JX0
