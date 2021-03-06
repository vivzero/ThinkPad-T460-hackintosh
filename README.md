# T460 hackintosh
![11](https://img.shields.io/badge/macOS-11-Green)

<details>
<summary><strong>Specs</strong></summary>
</br>

| Model | Lenovo 20FMS27120 |
| - | - |
| CPU | Intel Core i5-6300U |
| GPU | Intel HD Graphics 520 |
| RAM | 2x HMT451S6BFR8A-PB |
| SSD | THNSF5256GCJ7 (00PA997) |
| LCD | LP140WF6-SPF1 |
| Audio | Realtek ALC293 (ALC3245) |
| WLAN | Dual Band AC 8260 |
| BIOS | Latest |

</details>

<details>
<summary><strong>How to use it</strong></summary>
</br>

1. [Create a bootable installer](https://support.apple.com/en-us/HT201372)
1. Download this [EFI](https://github.com/vivzero/ThinkPad-T460-hackintosh/archive/refs/heads/main.zip) and extract it
1. Copy "EFI" folder, and paste it into ESP
1. Install
1. Enjoy

</details>

## Issues
- Bluetooth or Wi-Fi is not detected sporadically.
  * workaround: Restart your laptop.
- Sometimes Wi-Fi connection is lost after boot. (Itlwm)
  * workaround: Just wait.
- SD card reader doesn't work by default.
  * solution: [Sinetek-rtsx](https://github.com/cholonam/Sinetek-rtsx) works with `-rtsx_no_adma`, but It is disabled after wake.
- Function keys have no function.
  * solution: Use [YogaSMCNC](https://github.com/zhen-zen/YogaSMC/releases/download/1.5.1/YogaSMC-App-Release.dmg).
- Sometimes, NVMe drive (00PA997) causes kernel panic.
  * workaround: Use SATA drive.

</details>
