# Asrock Phantom Gaming ITX / 9900K / MSI v1 RX580

## Parts
* Intel Core i9-9900k
* ASRock Z390 Phantom Gaming-ITX/AC
* AMD RX580
* 16gb (2 x 8gb) Corsair Vengeance LPX DDR4 3200MHz
* AIO H100i Pro Liquid CPU Cooler
* Samsung 970 EVO 500gb - NVMe PCIe M.2.
* BCM94350ZAE WiFi + BT
* DA2 Streacom Mini-ITX Case

## What Works
* iGPU for Accelerated Graphics
* Airdrop
* Audio
* USB 3.0 Speeds
* Bluetooth
* Wi-Fi
* Ethernet
* Sleep
* Shutdown

## Still Testing
* iMessage (haven't checked)

## What doesn't work
* Thunderbolt Hot Plug
* Front Panel USB-C (SSDT may be out of date)

## Installation
* Will update eventually. If you'd like to know sooner, feel free to submit an issue.

### config.plist
* Be sure to generate a new `Serial Number` and `SmUUID` for the SMBIOS

### Motherboard
Currently using bios 1.50 with `Fix AsRock Z390 BIOS DSDT Device(RTC) bug` fix

Change these settings in the BIOS
* Advanced > Chipset Configuration > VT-d -> Disabled
* Advanced > USB Configuration > XHCI Hand-off -> Enabled

### Wi-Fi / Bluetooth 
* I replaced the stock Asrock Wi-Fi / BT card with a BCM94350ZAE WiFi / Bluetooth Chip.
