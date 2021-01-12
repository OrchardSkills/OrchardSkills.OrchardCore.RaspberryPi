# OrchardSkills.OrchardCore.RaspberryPi

Orchard Core on Raspberry Pi OS ARM 32bit

## Update the Raspberry Pi OS

```
sudo apt update
sudo apt full-upgrade
sudo reboot
```
## Update EEPROM

### Check if a update is needed

```
sudo rpi-eeprom-update
```

### Perform the update

```
sudo rpi-eeprom-update -a
```

## Clone the Orchard Skills RaspberryPi GitHub Repository

Launch Teminal

```
cd Documents/
mkdir GitHub
cd GitHub/
git clone https://github.com/OrchardSkills/OrchardSkills.OrchardCore.RaspberryPi.git
```

# Install VS Code

[.deb ARM](https://code.visualstudio.com/docs/?dv=linuxarmhf_deb)

Double click on downloaded file to install


## Install .NET Core 3.1

[.NET Core 3.1 SDK (v3.1.404) - Linux Arm32 Binaries](https://dotnet.microsoft.com/download/dotnet-core/thank-you/sdk-3.1.404-linux-arm32-binaries)

```
mkdir -p $HOME/dotnet && tar zxf dotnet-sdk-3.1.404-linux-arm.tar.gz -C $HOME/dotnet
```

Add the following to .bashrc file

```
export DOTNET_ROOT=$HOME/dotnet
export PATH=$PATH:$HOME/dotnet
```

## Configure Git

Replace FIRST_NAME LAST_NAME with your name. Replace MY_NAME@example with your email address.

```
git config user.name "FIRST_NAME LAST_NAME"
git config user.email "MY_NAME@example.com"
git config --global credential.helper store
```

# Push your first Commit

```
git commit -m "Commit initial code"
git push
username:
password:
```

## Install Microsoft Teams

[Microsoft Teams for Linux Releases](https://github.com/IsmaelMartinez/teams-for-linux/releases)

download teams-for-linux_1.0.5_armv7l.deb and install by double clicking on file

## Add C# extension in VS Code

## Customize Desktop

Click Raspberry Pi Icon -> Preferences -> Main Menu Editor

Select Preferences. Select Desktop Preferences, Desktop Session Settings, Display Settings, OpenBox Configuration Manager, Package Sources, Qt5 Settings, Setup Hot Keys, Theme and Appearance Settings

## Install more themes

```
sudo apt install arc-theme papirus-icon-theme breeze-cursor-theme -y
```

Seclect Preferences -> Theme and Appearance Settings

On Widgets Tab select Arc-Dark, On Icon Theme Tab select Papirus-Dark, On Mouse Cursor Tab select select Breeze, On Window Boarder select Arc-Dark and them pressed the Apply button.

Right Click on Panel and select Panel Settings. On Geometry Tab select Position Edge to Bottom. Increase the size of the icons Height to 48 and Width to 48. On the Panel Applets Tab click the Add button and add the CPU Temperature Monitor

## Add System Utilities (neofetch)

```
sudo apt install neofetch -y
```
## Modify config.txt

[Raspberry Pi Config.txt Settings](https://raspbian.org/RaspberryPiConfigTxt)

```
sudo nano /boot/config.txt
ctrl 0 ctrl x
```

```
hdmi_ignore_edid=0xa5000080
disable_overscan=1
```

Overclock Settings

```
over_voltage=6
arm_freq=2000
gpu_freq=750
```

# Install Argon One Case Drivers

```
curl https://download.argon40.com/argon1.sh | bash 
```
