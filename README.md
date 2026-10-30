# Ventoy-and-Persistence 
This tutorial guides you how to download ventoy, kubuntu and add persistance on a USB so it dosent change the Drive on your computer<br>
❗Not a tutorial to change or switch your main computer's OS❗<br>
Ventoy allows you to boot multiple operating systems (OS) from the same USB drive; it also allows you to add persistence (so you don't lose the changes that you make).<br>
```[NOTE] I wanted to put Ventoy and the 64-bit download of Kubuntu 26.04 LTS, including KDE Plasma for more customization options with persistence (persistence_ext4_4GB_casper-rw.dat.7z)```

## 📃Resources

* 32GB or larger
* 64-bit download of Kubuntu 26.04 LTS, including KDE Plasma : https://www.kubuntu.org/download/
* Ventoy2Disk.exe : https://www.ventoy.net/en/download.html
<br>  

## 🐾 Steps

### 1: Where are we putting it? on a USB!📍
I put mine on a USB Drive ✨, a 128GB USB drive specifically because I plan to put persistence and more than one OS on this USB drive.<br>
<img width="242" height="27" alt="image" src="https://github.com/user-attachments/assets/de1c1774-28c6-4e0d-90b0-d347d57d5250" /><br>
If you plan to use vento with or without persistence for 2 OS, the <u>minimum size needed is a 32GB USB. I recommend getting a 64GB drive or larger<u> as it will allow for more 🪱"wiggle" room if you were to add more operating systems or save files on the os using persistence; it's good to have extra space because we don't know exactly how much our system files, cache files, and pre-installed apps (if any) will take
```
[NOTE]
• Ventoy Installation: Takes only a tiny fraction of a megabyte.
• Two Operating System ISOs:
	• A typical Linux live ISO (like Linux Mint or Ubuntu) or Windows installer takes about 3 GB to 8 GB each.
	• Two OS ISOs will consume roughly 6 GB to 12 GB total.
• Persistence Files (.dat / .casper-rw):
	• Persistence files usually range from 2 GB to 8 GB (or larger) per operating system depending on how much
            personal data, apps, and settings you plan to save.
	• Two persistence files can easily take up 4 GB to 16 GB.
```
### 2: Downloading Ventoy on the USB📍
➖go to https://www.ventoy.net/en/download.html and download Ventoy2Disk.exe, ventoy-1.1.18-windows.zip
<img width="710" height="146" alt="image" src="https://github.com/user-attachments/assets/0fb4a481-fe20-49e5-8cd4-515876d4e767" /><br>
➖Extract the zip file
Double-click Ventoy2Disk (the application with the blue drive icon). 
<img width="852" height="410" alt="image" src="https://github.com/user-attachments/assets/0275a6a8-f5e0-4cd0-925f-5cddbaef0b90" /><br>
➖ Windows should asks, “Do you want to allow this app to make changes to your device?”, click Yes. The Ventoy window should open.<br>
➖Find the Device dropdown. Carefully select your USB drive. make sure its the right USB before proceeding. <br>
➖Click Install. Ventoy will warn you that the drive will be formatted.⚠️make sure no important info is on this USB vento will overwrite anything previously on the USB

