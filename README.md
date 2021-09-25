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
- SD card reader doesn't work by default.
  * solution: [Sinetek-rtsx](https://github.com/cholonam/Sinetek-rtsx) works with `-rtsx_no_adma`, but It is disabled after wake.
- Function keys have no function.
  * solution: Use [YogaSMCNC](https://github.com/zhen-zen/YogaSMC/releases/download/1.5.1/YogaSMC-App-Release.dmg).
- Bluetooth or Wi-Fi is not detected sporadically.
  * solution: Just restart, or replace WLAN card. (recommend DW1830: It is one of the M.2 cards with *BT 4.1*)

<details>
<summary>Catalina only (until commit 85c5ea6)</summary>
</br>

- System can't boot into macOS very occasionally.
- Hibernation (S4) doesn't work sometimes.
- Idle sleep doesn't work rapidly when AC is connected.
- It wakes from sleep after about 30 minutes, and doesn't sleep again.
  * workaround: Disable Power Nap.

</details>
