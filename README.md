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
