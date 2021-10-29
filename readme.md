# openSUSE Tumbleweed .NET 5 Yükleme
```
sudo zypper --gpg-auto-import-keys install -y libicu && sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc && wget https://packages.microsoft.com/config/opensuse/15/prod.repo && sudo mv prod.repo /etc/zypp/repos.d/microsoft-prod.repo && sudo chown root:root /etc/zypp/repos.d/microsoft-prod.repo && sudo zypper --gpg-auto-import-keys ref && sudo zypper --gpg-auto-import-keys in -y dotnet-sdk-5.0 
```


https://youtu.be/1PEgJ6lCwrA
