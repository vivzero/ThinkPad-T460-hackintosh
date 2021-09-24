# T460 hackintosh
![10.15](https://img.shields.io/badge/macOS-10.15-green)

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
1. Install (with twice of rebooting)
1. Enjoy

</details>

## Issues
- System can't boot into macOS very occasionally.
- Bluetooth or Wi-Fi is disabled after boot very occasionally.
- Hibernation (S4) doesn't work sometimes.
- Idle sleep doesn't work sometimes.
- kernel panic occurs sometimes when wake from idle sleep. (IONVMeFamily)
- It can sleep but wakes after about 30 minutes, and doesn't sleep again.
  * workaround: Disable Power Nap.
- Function keys have no function.
  * solution: Use [YogaSMCNC](https://github.com/zhen-zen/YogaSMC/releases/download/1.5.1/YogaSMC-App-Release.dmg).
- [Sinetek-rtsx](https://github.com/cholonam/Sinetek-rtsx) works with `-rtsx_no_adma`, but It doesn't work after wake. (*Disabled by default*)
  * workaround: Using `rtsx_sleep_wake_delay_ms=1000` will be helpful.

I think that Itlwm and IntelBluetooth kexts are one of the causes..