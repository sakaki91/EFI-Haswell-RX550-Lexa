# EFI OC Haswell + RX550 Lexa 4GB (Metal2)

<p>
<b>Build:</b><br>
Mobo: Kingster H81 1150 DDR3<br>
CPU: Intel Core i5-4590 3.70GHz<br>
Ram: 16GB Dual-Channel Kingston DDR3 1600MHz<br>
Storage: 256GB NVME<br>
GPU: Mancer RX550 Lexa 4GB<br>
<br>
<b>Compatible Versions:</b><br>

macOS Catalina (10.15): ✅, Good and consistent performance.<br>
macOS Bigsur: ✅, Good and consistent performance. (RECOMMENDED!).<br>
macOS Monterey: ✅, Good performance.<br>
macOS Ventura: ✅, Performance OK, but very usable.<br>
macOS Sonoma: ⚠️, Usable, but with much of the performance compromised by the absence of Metal 3 on the GPU.<br>
macOS Sequoia: ⚠️, Usable, but with much of the performance compromised by the absence of Metal 3 on the GPU.<br>
<br>

<b>Tutorial:</b>

Open the terminal and type:<br>
**`diskutil list`** - this will list all your disks<br><br>
**`sudo diskutil mount /dev/yourdisk`** - this will mount your efi partition according to your disk (e.g. /dev/disk0s1)<br>
<br>After that, just delete the old EFI and move the new one to the partition, and you're done!<br>
You have a working Hackintosh Haswell with RX550 Lexa
<br><br>
<b>Important Links:</b><br>
<a href=https://olarila.com>Olarila</a><br>
<a href=https://dortania.github.io>Dortania</a>
<br>

<b>Working Setup:</b><br>
![Working Setup:](example.png)
<p>
