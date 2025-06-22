# Linux-Mint-Install-Repo

A short Cheat Sheet for setting up Linux Mint to my own preferences and tools / drivers / ...

## Prepare

1. Install Mint using the official installer and documentation

2. Go threw the welcome menu and setup all your preferences.

3. Update system

4. Do Timeshift INIT Backup and Schedule

## Installation of Tools

Grab the latest DEBs of Proton and install them.

**GenPurp**:

```bash
sudo apt install  spotify-client gnome-builder calibre gimp gimp-help-de darktable handbrake obs-studio vlc filelight baobab python3-virtualenv python-pip python3 glances most dia ghex tree bleachbit ipython3 neofetch gnome-keyring android-sdk-platform-tools-common qbittorrent openssh-client chromium
```

**Optional**:

Games:

```bash
sudo apt install dolphin steam-installer gnome-games lutris
```

Misc:

```bash
sudo apt install burp nmap wireshark hashcat virtualbox virtualbox-ext-pack 
```

**Flatpak**:

```bash
sudo flatpak install com.github.marktext.marktext
sudo flatpak install md.obsidian.Obsidian 
sudo flatpak install com.vscodium.codium
sudo flatpak install org.ghidra_sre.Ghidra
sudo flatpak install appimage-pool
sudo flatpak install com.github.tchx84.Flatseal
sudo flatpak install flathub org.signal.Signal
sudo flatpak install org.jdownloader.JDownloader
```

**Jetbrains**

[Download PyCharm 2025.1.2](https://www.jetbrains.com/shop/download/PC/2025100)

**IDA Free**

[My Hex-Rays Account](https://my.hex-rays.com/dashboard/download-center/installers/9.1/ida-free)

## Post install

```bash
#Prepare Graphe Plugin for IDA-free
git clone https://github.com/WqyJh/qwingraph_qt5.git
cd qwingraph_qt5
sudo ./install.sh
rm -rf qwingraph_qt5

ssh-keygen -t rsa -b 4096 -o -a 100
```

Open Software Center and enable Flatpak unsigned in settings two find more Flatpaks 

## Performence

```bash
sudo apt install preload tlp tlp-rdw
sudo systemctl enable tlp --now
sudo systemctl enable fstrim.timer --now
```

## Terminal Tweaks

```bash
echo "export PAGER=most" >> ~/.bashrc
```

**Gogh**

```bash
bash -c "$(curl -sLo- https://git.io/vQgMr)"gpar
```
