# T460 hackintosh
- Supported OS: Catalina

## Specs
- CPU: Intel Core i5-6300U
- GPU: Intel HD Graphics 520
- LCD: LP140WF6-SPF1
- RAM: HMT451S6BFR8A-PB
- SSD: THNSF5256GCJ7
- WLAN: Dual Band AC 8260
- Audio: Realtek ALC293
- BIOS: Latest

## Setup configs
- Disable secure boot
- Disable FP, SC, and SD for saving power
- Disable useless items (i.e. AT, AMT, TPM, etc.) (*Optional*)

## Issues
- [Sinetek-rtsx](https://github.com/cholonam/Sinetek-rtsx) works with `-rtsx_no_adma`, but It has low speed and does not work after wake (disabled by default)
- ~~A prohibitory symbol displays very occasionally when booting.~~
- Hibernation fails sometimes.
- standby (S3 to S4) doesn't work, just keeps S3 mode?
