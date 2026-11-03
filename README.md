# Ventoy-and-Persistence 
This tutorial guides you on how to download Ventoy, Kubuntu, and add persistence to a USB on Windows 11 so it doesn't change the Drive on your computer. <br>
❗Not a tutorial to change or switch your main computer's OS❗<br>
Ventoy lets you boot multiple operating systems (OS) from the same USB drive; it also lets you add persistence (so you don't lose the changes you make).<br>
```[NOTE] I wanted to put Ventoy and the 64-bit download of Kubuntu 26.04 LTS, including KDE Plasma for more customization options with persistence (persistence_ext4_4GB_casper-rw.dat.7z)```

## 📃Resources

* 32GB USB or larger
* 64-bit download of Kubuntu 26.04 LTS, including KDE Plasma : https://www.kubuntu.org/download/
* Ventoy2Disk.exe : https://www.ventoy.net/en/download.html
<br>  

## 🐾 Steps

### 1: Where are we putting it? On a USB!📍
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
	• Persistence files usually range from 2 GB to 8 GB (or larger) per operating system, depending on how much
            personal data, apps, and settings you plan to save.
	• Two persistence files can easily take up 4 GB to 16 GB.
```
### 2: Downloading Ventoy on the USB📍
➖go to https://www.ventoy.net/en/download.html and download Ventoy2Disk.exe, ventoy-1.1.18-windows.zip
<img width="710" height="146" alt="image" src="https://github.com/user-attachments/assets/0fb4a481-fe20-49e5-8cd4-515876d4e767" /><br>
➖Extract the zip file. Then, in the extracted file
Double-click Ventoy2Disk (the application with the blue drive icon). 
<img width="852" height="410" alt="image" src="https://github.com/user-attachments/assets/0275a6a8-f5e0-4cd0-925f-5cddbaef0b90" /><br>
➖ Windows should ask, “Do you want to allow this app to make changes to your device?” Click Yes. The Ventoy window should open.<br>
➖Find the Device dropdown. Carefully select your USB drive. Make sure it's the right USB before proceeding. <br>
➖Click Install. Ventoy will warn you that the drive will be formatted.⚠️ Make sure no important info is on this USB; Ventoy will overwrite anything previously on the USB<br>
<img width="541" height="430" alt="image" src="https://github.com/user-attachments/assets/8639ed6d-1477-45fa-8317-82dd4153996b" /><br>
<br>
```
[NOTE]
• Ventoy will create two partitions on your USB

• Partition 1 (Main Partition): Formatted as exFAT (by default) or another filesystem like NTFS, FAT32, or Ext4.
This is the large partition where you drag and drop your ISO, WIM, IMG, or VHD files

• Partition 2 (Ventoy Boot Partition): A small hidden or system partition (usually around 32MB) that holds the EFI bootloader
and necessary Ventoy files required to boot your machine

More info on: https://www.ventoy.net/en/doc_disk_layout.html
```
<img width="1112" height="462" alt="image" src="https://github.com/user-attachments/assets/3caa0d51-4777-4feb-aced-841070aca262" /><br>
⚠️DO NOT COPY KUBUNTU INTO VTOYEFI (E:) PARTITION OF DRIVE<br>

### 3: Next, we'll download the Kubuntu ISO and copy it to the USB D:📍
➖ go to https://kubuntu.org/id/download/ to download kubuntu-26.04.1-desktop-amd64.iso<br>
➖Save it to your Windows computer's Downloads folder first<br>
➖ Then copy it to your USB<br>
<img width="1347" height="540" alt="image" src="https://github.com/user-attachments/assets/4c4ee100-f882-48ef-a80d-040567da2ba5" />


### 4: Then configure persistence so your KDE customizations and files survive reboots.📍
➖Go back to the folder where you extracted ventoy-1.1.18-windows.<br>
➖Double-click VentoyPlugson.exe, and if Windows asks for permission, click Yes.<br>
➖it should open the following popup:<br>
<img width="441" height="157" alt="image" src="https://github.com/user-attachments/assets/31f4f1c0-84f1-4959-9102-01f28d80d61e" /><br>
➖Click start<br>
➖Then it should open a browser page for configuring Ventoy plugins.<br>
<img width="1911" height="925" alt="image" src="https://github.com/user-attachments/assets/a173e03c-cf70-49c1-8c47-16f5be95ac43" /><br>
➖Click Persistence Plugin in the left sidebar, near the middle of the page.<br>
<img width="1917" height="925" alt="image" src="https://github.com/user-attachments/assets/a6abb619-31c2-4b4b-a88f-587a452763a5" /><br>
➖Click the green + Add button on the right side of the table. (This should open a row or form for the persistence settings)<br>
<img width="772" height="396" alt="image" src="https://github.com/user-attachments/assets/6fb70bc2-f573-40a1-8e6c-4f4fb2d809ca" /><br>
➖ Paste the file path to Kubuntu into the file path <br> it should look something like D:\kubuntu-26.04.1-desktop-amd64.iso<br>
➖ Don't click OK yet; we have to add the persistence file<br>
➖A file named CreatePersistentImg.cmd should have been in the file ventoy-1.1.18-windows that we extracted earlier
 But I couldn't find it, so I had to go to the official Ventoy persistence backend releases<br>
 https://github.com/ventoy/backend/releases<br>
➖look for the file named persistence_ext4_4GB_casper-rw.dat and download that (download images.zip file)<br>
<img width="125" height="27" alt="image" src="https://github.com/user-attachments/assets/ba6acc4d-045b-453f-83cf-fe9e0200ca3c" /><br>
➖i had to create a file to extract the persistence_ext4_4GB_casper-rw into, because it wasent showing up in my downloads after extracting it "normaly" onto my downloads<br>
➖Right-click persistence_ext4_4GB_casper-rw.dat and select Copy.<br>
➖Then Paste the file directly into the main Ventoy (D:) drive, alongside your Kubuntu ISO and the ventoy folder.<br>
➖in the Dat file underneth the file path put the path to your persistance file within the USB D: drive (For Example: D:\persistence_ext4_4GB_casper-rw.dat)<br>
➖once you have both paths correct click okay then go to preview<br>
➖the preview should look something like this:<br>
<img width="1537" height="792" alt="image" src="https://github.com/user-attachments/assets/5cfefdcd-90f6-403a-99b5-0aba174f53e4" /><br>
```you can also  Verify the configuration before booting Kubuntu on the usb
• In the ventoy folder, right-click ventoy.json. Choose Open with → Notepad. Look for the persistence section.
• It should contain your Kubuntu ISO and persistence file paths, similar to this:

{
    "persistence": [
        {
            "image": "/kubuntu-26.04.1-desktop-amd64.iso",
            "backend": [
                "/persistence_ext4_4GB_casper-rw.dat"
            ]
        }
    ]
}
``` 
➖Close the Plugson page. 
➖If the Ventoy Plugson program is still open on your desktop, close that window too
➖Safely eject the USB from the Windows taskbar
❗Leave the SanDisk USB plugged into your computer after saftely ejecting it❗
<br>
### Booting Kubuntu with persistance from USB
➖after saftely ejecting the usb depending on what computer you have you will have to get to the BOOT Menue 
```i have a NIMO laptop running win11 so i had to restart my computer and repediatly press F12 after the screen went dark to get to the BOOT Menu```
➖
<img width="1536" height="1152" alt="image" src="https://github.com/user-attachments/assets/ba00b5ba-4f66-467a-bcc0-5f7b71a6ec29" />
<img width="1536" height="1152" alt="image" src="https://github.com/user-attachments/assets/1acda80f-637e-4eeb-837a-9e88c5f20689" />
press any key once to open MOK management.
Choose “Enroll key from disk.”



