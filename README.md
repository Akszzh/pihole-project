# pihole-project
My Pi-hole setup using Raspberry Pi Zero to block ads on a local network.

This is my personal project where I installed Pi-hole on a Raspberry Pi Zero 2 W to block ads and trackers on all devices connected to my hotspot network.

## 🖥️ Hardware Used
- Raspberry Pi Zero 2 W
- 16GB Micro SD card
- Mobile Hotspot (for internet)
- USB power adapter
- Laptop (to configure Pi-hole) and it also provide internet for Raspberry pi zero 2w

## 🛠️ Software Used
- Raspberry Pi OS Lite
- Pi-hole (installed via curl script)
- SSH (for remote setup)

## 🔧 Installation Steps
1. Installed Raspberry Pi OS using Raspberry Pi Imager
2. Connected Pi to Wi-Fi via `raspi-config`
3. SSH into Pi from my laptop using pi ip address
4. Installed Pi-hole:
comment to install pi hole:
curl -sSL https://install.pi-hole.net | bash
5. Set a static IP to raspberrypi in my router
6. Opened Pi-hole admin page at `http://<Pi-IP>/admin`
7. Disabled Private DNS on mobile to make it work

## 🛠️ Issues I Faced and Fixed
- Pi-hole showed 0 queries at first
  - ✅ Fixed by disabling Private DNS on Android
- Couldn't resolve domains
  - ✅ Fixed by setting a temporary DNS in `/etc/resolv.conf`
 
 ## 🚀 Future Plans
- Add unbound for DNS encryption
- Use battery backup for portability
- Add more custom blocklists

  ## 📸 Screenshots
  ![Pi-hole Dashboard](Screenshot%202025-06-30%20192611.png)



