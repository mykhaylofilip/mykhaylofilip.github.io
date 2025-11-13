<link rel="stylesheet" href="/assets/css/custom.css">

# Simple Firewall Setup on Linux
I wanted to set up a basic firewall on my Linux machine. Using `ufw` (Uncomplicated Firewall), I was able to block unnecessary ports and allow only the services I need, like SSH and HTTP.

The commands are simple:
```
sudo ufw enable
sudo ufw allow ssh
sudo ufw allow 80/tcp
sudo ufw status
```
After enabling it, I noticed my system was more secure without any extra software. A firewall is a good first step in protecting a personal or lab environment.

[UFW Documentation](https://help.ubuntu.com/community/UFW)
