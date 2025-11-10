# Kali Linux on ARM Devices
I experimented with installing Kali Linux on a Raspberry Pi 4B. ARM builds have improved dramatically over the years, offering full Kali toolsets without major compromises. The key is to use a lightweight desktop environment, like XFCE, to minimize CPU strain.

After flashing the SD card with Kali ARM image, I updated repositories and installed my common pentesting tools. Performance-wise, it handled Nmap scans, Wireshark captures, and small password cracking tasks surprisingly well. However, for GPU-intensive work like hashcat, ARM devices fall short.

This setup is perfect for a portable penetration testing rig. It’s light, battery-powered, and ideal for network reconnaissance. Pairing it with an external SSD instead of an SD card also improves speed and reliability.

For anyone interested in mobile labs, ARM devices running Kali are becoming increasingly practical.

[Kali ARM Images](https://www.kali.org/get-kali/#kali-arm)
