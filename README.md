# RiiConnect24 DNS Server [![Actions Status](https://github.com/RiiConnect24/DNS-Server/workflows/CI/badge.svg)](https://github.com/RiiConnect24/DNS-Server/actions)

This DNS Server will run locally on your computer and allow your Wii to connect to RiiConnect24 servers even if your ISP blocks connections to our DNS Server.

## Setup

Setup process is the same as shown on our guide
https://wii.guide/riiconnect24 

You will only need to change DNS Settings in your Wii.

First, make sure that your Wii is connected to the same network as your computer is.

# Running on Windows:

Run the .exe provided [on this site](https://github.com/RiiConnect24/RiiConnect24-DNS-Server/releases). If your antivirus notifies you about the .exe file, allow it and run it. If it doesn't work, you should also allow communication for this this .exe in your firewall settings.

# Running on Linux/macOS:

You will need to install Python 3 and run these commands in the Terminal.

> pip install dnslib requests

To run it, simply type in:

> sudo python3 RiiConnect24-DNS-Server.py

Replace `python3` with the name/path to your Python binary if necessary

# How to use it?

After starting the program, it will download the current list of the DNS Addresses to forward and will run. 

On screen, you will see the IP Address assigned to your computer by the DHCP Server on your NAT (router).

If your Wii is connected to the same network as your PC, it will be able to connect to the server on your PC.

<p align="center">
  <img src="https://i.imgur.com/oageZQ3.jpg">
<i>My local IP Address, yours will be different.</i>
</p>


# Compiling on Windows

To compile this app on Windows, you will need to run these two commands:
>pip install dnslib requests pyinstaller

Once it's done installing, run:
>pyinstaller RiiConnect24-DNS-Server_v1.0.spec


| Tip: You may need to edit RiiConnect24-DNS-Server_v1.0.spec so compiling process works on your computer.

# Need more help?
You can talk to us over on the [RiiConnect24 Discord server](https://discord.gg/b4Y7jfD), where people can try and help you out!
