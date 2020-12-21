# OrchardSkills.OrchardCore.RaspberryPi

Orchard Core on Raspberry Pi OS 64bit

## Update the Raspberry Pi OS

```
sudo apt update
sudo apt full-upgrade
sudo reboot
```

# Install VS Code

[.deb ARM64](https://aka.ms/linux-arm64-deb)

Double click on downloaded file to install


## Install .NET Core 3.1

[.NET Core 3.1 SDK (v3.1.404) - Linux Arm64 Binaries](https://download.visualstudio.microsoft.com/download/pr/de47cbe2-f75f-44c5-8250-7960a36d6591/76cfdbfb7bf17cce27378a9fddd969a6/dotnet-sdk-3.1.404-linux-arm64.tar.gz)

```
mkdir -p $HOME/dotnet && tar zxf dotnet-sdk-3.1.404-linux-arm64.tar.gz -C $HOME/dotnet
```

Add the following to .bashrc file

```
export DOTNET_ROOT=$HOME/dotnet
export PATH=$PATH:$HOME/dotnet
```

## Configure Git

```
git config user.name "FIRST_NAME LAST_NAME"
git config user.email "MY_NAME@example.com"s
git config --global credential.helper store
```