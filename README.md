# Asrock Phantom Gaming ITX / 9900K - Opencore Installation
* Version - 10.15.6
* The kexts have been updated to support MacOS Catalina! Do a fresh install of all kexts to be safe. (Including removing those added to other folders not in `EFI`)

##### Table of Contents
* [Images](#images)
* [PC Parts](#parts)
* [BIOS Settings](#bios)
* [What Works](#what-works)
* [Installation](#installation)
* [Motivation](#motivation)

<a name="images"></a>

## Images

![About this Mac](./images/catalina-10-15-screenshot.png?raw=true)

![Desktop Screenshot](./images/neofetch.png?raw=true)

<div align="center">
  <img src="images/catalina-geekbench.png?raw=true">
</div>


### PC: Photos out of Date
![PC Case - Side Closed](./images/closed-side-pc.jpg?raw=true)
![PC Case - Front](./images/front-pc.jpg?raw=true)
![PC Case - Back](./images/back-pc.jpg?raw=true)
![PC Case - Open Side Left](./images/open-pc-side-left.jpg?raw=true)
![PC Case - Open Side Right](./images/open-side-pc-right.jpg?raw=true)

<a name="parts"></a>

## Parts
* Intel Core i9-9900k
* ASRock Z390 Phantom Gaming-ITX/AC
* AMD Sapphire RX570
* 16gb (2 x 8gb) Corsair Vengeance LPX DDR4 3200MHz
* Noctua NH-DL9
* Samsung 970 EVO 500gb - NVMe PCIe M.2.
* WD Blue 3D NAND 1TB PC SSD
* Broadcom BCM94352Z (Dell DW1560)
* DA2 Streacom Mini-ITX Case

<a name="bios"></a>

## BIOS - TBD

<a name="what-works"></a>

## What Works
* ~~iGPU for Accelerated Graphics~~
* Airdrop
* Audio
* USB 3.0 Speeds
* iMessage
* Bluetooth
* Wi-Fi (2.4 and 5ghz)
* Ethernet
* Sleep (have not had issues for the past few months! As of 10/26/2019)
* Shutdown
* Front Panel USB-C
* Thunderbolt 3 (for graphics or for usb when powered on with it)

<a name="installation"></a>

## Installation
* It is HIGHLY recommended you read through the [Open Core Install Guide](https://dortania.github.io/OpenCore-Install-Guide/) before using this repository. There's no guarantee that the way I've set this up will work for your machine and you may need to tweak bios settings, kexts, etc.

### config.plist
* Be sure to generate a new `MLB`, `Serial Number` and `SmUUID` for the SMBIOS. Opencore has details on this as well

### Wi-Fi / Bluetooth 
* ~~I replaced the stock Asrock Wi-Fi / BT card with a BCM94350ZAE WiFi / Bluetooth Chip. (create an issue if you'd like more documentation on this process)~~
* [Moved to this card](https://www.ebay.com/itm/252319175707) - I've tested 5ghz and BT on both MacOS and Windows and each works without a problem as of **6/07/2019**

<a name="motivation"></a>

## Why I Decided to Build a Hackintosh
My reasons for using macOS are pretty straightforward: I am a developer that loves MacOS for the look and feel of the operating system, and also MacOS' UNIX development environment. Anything outside of the MacPro will run hot and slower than a desktop PC unfortunately. Opencore is surprisingly easy to setup, and works pretty smoothly, even in beta.
