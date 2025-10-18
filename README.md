# EFI OC Haswell + RX550 Lexa 4GB (Metal2, Full-support with DRM and Encoders!)

<p>
<b>Build:</b><br>
Mobo: Kingster H81 1150 DDR3<br>
CPU: Intel Core i5-4590 3.70GHz<br>
Ram: 16GB Dual-Channel Kingston DDR3 1600MHz<br>
Storage: 256GB NVME<br>
GPU: Mancer RX550 Lexa 4GB<br>

This setup works from macOS Catalina to macOS Sequoia with decent performance between versions.  

- [Tutorial](#tutorial)
- [Modifications](#modifications)
- [Important Links](#important-links)
- [Screenshot](#working-setup)
### <b>Tutorial:</b>

Open the terminal and type:<br>
**`diskutil list`** - this will list all your disks<br><br>
**`sudo diskutil mount /dev/yourdisk`** - this will mount your efi partition according to your disk (e.g. /dev/disk0s1)<br>
<br>After that, just delete the old EFI and move the new one to the partition, and you're done!<br>
You have a working Hackintosh Haswell with RX550 Lexa
<br><br>

### <b>Modifications:</b>

<b>boot-args:</b>  

    -v alcid=1 watchdog=0 agdpmod=pikera dk.e1000=0 e1000=0 shikigva=80 unfairgva=1 -radcodec

<b>SMBIOS:  
Has a Generic Serial (macmini8,1) and you need to regenerate a new SMBIOS using [genSMBIOS](https://github.com/corpnewt/GenSMBIOS)</b>

<b>Kexts present:</b>  

    Lilu.kext 
    VirtualSMC.kext
    AirportBrcmFixup.kext
    AppleALC.kext
    AtherosE2200Ethernet.kext
    IntelMausi.kext
    RealtekRTL8111.kext
    RestrictEvents.kext
    SMCProcessor.kext
    SMCSuperIO.kext
    USBInjectAll.kext
    WhateverGreen.kext

<b>PCI/GPU-Setup:</b>

    Key: AAPL,slot-name | Value: Internal@0,3,1/0,0/0,0/0,0 | Type: STRING
    Key: device-id | Value: FF670000 | Type: DATA
    Key: device_type | Value: VGA compatible controller | Type: STRING
    Key: hda-gfx | Value: onboard | Type: STRING
    Key: model | Value: Radeon RX550 | Type: STRING
    Key: no-gfx-spoof | Value: 01000000 | Type: DATA

<b>ACPI:</b>  
This EFI uses MaLd0n and Dortania SSDT's profiles  

    MaLd0n.aml
    SSDT-PLUG-DRTNIA.aml
### <b>Important Links:</b><br>
<a href=https://olarila.com>Olarila</a><br>
<a href=https://dortania.github.io>Dortania</a><br>
<a href=https://github.com/corpnewt/GenSMBIOS>genSMBIOS</a><br>  
### <b>Working Setup:</b><br>
![Working Setup:](example.png)
<p>
