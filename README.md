# FM06: Drone Mitigation
###### Brandon Duong, Muzammil Shaikh, Regan Ly
## Table of Contents
* [Abstract](#Abstract)
* [Basic Methodology](#Basic-Methodology)
* [Components](#Components)
* [Installation](#Installation)
* [Usage](#Usage)

## Abstract
Today’s commercially available drones can fly for miles and can take video, pictures and audio from a target. These drones mostly work in usual unlicensed spectrum of 2.4GHz or 5GHz similar to Wi-Fi. Many of them use frequency hopping to prevent jamming and to improve Signal to Noise (S/N) ratio. The required system must first listen to these unlicensed frequency range and detect drones that are communicating in this frequency range. Then it must track the frequency hopping and must send a pulse of noise for each hopped frequency to reduce S/N ratio so that the drone can’t communicate with its controller.
## Basic Methodology
* Put the pseudocode here
## Components
* `Raspberry Pi 3 B+` : Low cost computer that will be the hub to all the other devices purchased for the project. Must be wifi compatible and have USB ports and an SD card port.  We chose to purchase the B+ version over the B version because the prices are almost identical and the B+ version supports gigabit ethernet and dual-band 802.11ac wifi.
* `16GB microSD Card` : If using a Raspberry Pi 3 B+ as the controller, a microSD card will be needed in order to boot Linux. Linux only requires around 1.9 GB, but the recommended capacity of the microSD card when paired with the Raspberry Pi is 16 GB. Therefore, a 16 GB microSD card will be purchased.
* `Wireless Network Adapter (For Hacking): ` :Any ordinary wireless network adapter can connect to a wireless network, but this project requires an adapter that supports packet injection (packet spoofing) and monitor mode in order to achieve wifi hacking. Packet injection is the process of forging packets into a network connection to intercept +communication. It is the main process in DoS attacks. Monitor mode allows the adapter to passively listen and monitor to all packets (traffic) on a specific channel. Typical adapters only operate in managed mode (status infrastructure mode), whose purpose is to just connect to specific networks. A popular adapter for hacking that we found is the **Alfa AWUS036H**.
* `Wireless Network Adapter (For Connectivity)` : Will connect to the Raspberry Pi via USB. Its purpose is to launch a network that can be connected to from a secondary device, such as a smartphone. This will allow us to control drones through a mobile application. The **Edimax EW-7811Un** is low cost and provides the functions that we need.
* `Batteries` : An important aspect of the hardware portion is keeping the system portable, so the USB battery should be fairly light. Also, that means if there is a  microcontroller that is doing hacking or even if is being done in an app, there needs to be a power supply. Having a power supply keeps the project realistic as then the hardware is mobile and can be brought from one place to another without interruption. Not to mention, if the hardware requires to be in an “Auto-pilot” there the hardware would be running nevertheless. From viewing some common microcontrollers, Espruino runs at 32mA, Arduino at about 42mA and Raspberry PI’s run from 80-220mA. Even with the Raspberry PI’s the developers claimed that they could run on a 1400mAh battery pack for four hours continuously. This means that anything running low power such as any of the other microcontrollers will be able to run for a long time without being shut off. A 2000mAh battery pack costs about 15 dollars and can be as small as 10cm by 5cm (Already have.)

| BOM Level | Part Number    | Part Name | Quantity | Total Cost |
| --------- | ---------------| --------- | -------- | ---------- |
| 1 | 9001 | Raspberry Pi 3 B+ | 1 | 70.22 |
| --------- | ---------------| --------- | -------- | ---------- |
| --------- | ---------------| --------- | -------- | ---------- |
| --------- | ---------------| --------- | -------- | ---------- |
| --------- | ---------------| --------- | -------- | ---------- |

## Installation
## Usage
* Explain the code here, doesn't have to be too in depth
