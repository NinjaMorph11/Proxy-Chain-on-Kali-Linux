# Proxy-Chain-on-Kali-Linux
I'm making a Proxy to protect myself from getting detected whenever I do Ethical Hacking in Kali Linux

Why?

Now to make this short and simple, doing a simple scan using Nmap can expose ourselves on the internet. We can get detected and go to jail. 

What's the solution? 

Set up a proxy server. A proxy allows our data to be sent to a middle man instead of straight away to the victim. So when the victim wants to check the IP Address of the attacker, it will be the middle man, which is the proxy server.

However?

However the victim or the investigator might still find out who you are because when they look and contact the Proxy Server's IP Address. They can find logs which will eventually lead them to us.

How do we counter this? Or make it harder?

We do "Proxy Chaining", this means instead of sending the attack to one proxy server, we send it to multiple proxy servers. Making it harder for the investigators to find out who attack the victim.

In Linux

Type command "locate proxychain"

Locate the file called proxychains.conf



Skip

To test out if our proxychains work.

Command:
proxychains firefox google.com

Upon trying to connect to google, I couldn't.

Due to the fact that WiFi wasn't working in my Kali Linux.

1. sudo su
2. service NetworkManager status
3. [CTRL + C]
4. service NetworkManager restart

At this point it should solve the problem, but if it didn't, then follow these steps.
You might need to install the server

1. apt-get update
2. apt-get dist-upgrade

Now you have to reboot your system.

1. reboot

Now if the network icon is still not appearing. 

1. sudo su
2. cd Desktop
3. apt install git
4. git clone https://github.com/TadakaSuryaTeja/BroadcomInstaller2021.git
5. ls to check if BroadcomInstaller2021 is there
6. cd BroadcomInstaller2021
7. chmod +x Broadcom.sh
8. ls to see if Broadcom.sh is there
9. ./Broadcom.sh to open the wifi installer
10. Enter 1
