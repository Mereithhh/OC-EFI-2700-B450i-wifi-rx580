# OC-EFI-2700-B450i-wifi
OpenCore Hackintosh EFI, Based on GIGABYTE B450i wifi,AMD 2700,RX580 4G<br><br>

if you have similar hardware with me, you can have a try.<br><br>

**updated: 2020/03/26**<br>
**oc:     0.5.6** <br>

## hardware

| Device | Model |
| :--:   | :--:  |
| CPU    | amd 2700 |
| GPU    | RX580 4G |
| Motherboard | GIGABYTE B450i wifi pro |
| RAM | Kingston Predator DDR4 3000 16Gx2 |
| NVME SSD |  Hikvision C2000 1TB |

## How to use?

1. Download this ,extract the `EFI` folder in a USB disk (FAT32) or  the EFI partition on your local disk. <br><br>

2. update your BIOS if you need,you can use the update file in the `bios_update` folder in this project<br><br>

3. open your BIOS,and set as follow:<br><br>

**Disable:**<br><br>

* Fast Boot<br>
* CSM(if you can't turn it off,ignore it)<br>
* Above 4G decoding **IMPORTENT!**<br>

**Enable**<br><br>

* EHCI/XHCI Hand-off<br><br>

4. Select the boot device which the `EFI` folder we just copy inside.<br><br>

5. enjoy! if something is wrong ,you can add `-v` in `boot-args` of the `config.plist` under `EFI/OC` folder.

##  One more thing

if you have trouble , you can read the [troubleshooting]() ,and most of the issues can be fixd.<br><br>

in fact , i made this by reading [Opencore Vanilla Desktop Guide](https://khronokernel.github.io/Opencore-Vanilla-Desktop-Guide/), you can also make your own EFI by yourself.
<br><br>

i will update my EFI time to time , both kexts、 efi drivers and opencore will be updated togethor.<br><br>

## PS

* wifi and bluetooth can't work! (intel just can't)<br>