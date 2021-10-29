# OpenSUSE Tumbleweed Nvidia Driver yükleme

##Nvidia G05
> GeForce 600 serisi ve daha yenisi için NVIDIA grafik sürücüsü
```
sudo zypper --gpg-auto-import-keys addrepo --refresh https://download.nvidia.com/opensuse/tumbleweed NVIDIA && sudo zypper --gpg-auto-import-keys ref && sudo zypper --gpg-auto-import-keys in x11-video-nvidiaG05 nvidia-glG05
```

##Nvidia G04
> GeForce 400 serisi ve daha yenisi için NVIDIA grafik sürücüsü
```
sudo zypper --gpg-auto-import-keys addrepo --refresh https://download.nvidia.com/opensuse/tumbleweed NVIDIA && sudo zypper --gpg-auto-import-keys ref && sudo zypper --gpg-auto-import-keys in x11-video-nvidiaG04 nvidia-glG04
```

https://youtu.be/Hjm5f9sj-rs
