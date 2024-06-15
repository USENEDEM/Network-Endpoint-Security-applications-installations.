# Network-Endpoint-Security-applications-installations.
---
### Preview
---

This project gives more insight and practical analysis on installation and configuration of network security applications.

### Skills ( Learned )
---
### *Bullet points*

1. Installation and configuration of firewall software(pf sense).
2. Installation and configuration of intrusion detection systems (snort).
3. Installation and configuration of data encryption and anonymity software (protonvpn).
4. Endpoint protection / security.

### Tools
___

1. Pfsense firewall - For filtering inbound and outbound traffic in the *DMZ* [Download here](https://www.pfsense.org/download)
2. Snort - Intrusioon detection system
3. Protonvpn - Data encryption and anonymity [Download here](https://www.protonvpn.com)
4. Kali linux - Debian based operating based operating system [Download here](https://www.kali.org)
5. Oracle virtual box - Virtualization software [Download here](https://www.virtualbox.org)

### Procedures
---
### Pfsense

1.Downloaded the pfsense community edition by creating an account on the pfsense netgate website.Selected the *AMD 64 iso* file for virtual machines as it is going to be installed on my virtual box.


<img width="1280" alt="Screenshot 2024-05-24 at 15 36 58" src="https://github.com/USENEDEM/Network-Endpoint-Security-applications-installations./assets/169564406/17fa1b58-a18f-452f-a072-f15ce576db87">

*Ref. 1* (Create account)


<img width="1280" alt="Screenshot 2024-05-24 at 15 35 49" src="https://github.com/USENEDEM/Network-Endpoint-Security-applications-installations./assets/169564406/4e09327b-9ee4-4afa-b367-a772ff31574f">

*Ref. 2* (Selecting *AMD 64 Iso* file)

2. I Clicked on the *new* icon to add the pfsense as a new machine on virtual box, added the *Iso* file and selected the *freeBSD* operating system.Created a hard disk , set up network interface and started up the machine to complete the configuration before rebooting using *ZFS* for disk partitioning.


<img width="1280" alt="Screenshot 2024-05-26 at 04 13 08" src="https://github.com/USENEDEM/Network-Endpoint-Security-applications-installations./assets/169564406/2b60ae68-6f72-4dc6-a386-d87849fc68b4">

*Ref 3.* (Setting up network)


<img width="1280" alt="Screenshot 2024-05-24 at 17 28 31" src="https://github.com/USENEDEM/Network-Endpoint-Security-applications-installations./assets/169564406/59a898eb-8166-476e-91d6-ccbb7661ea1c">


*Ref 4.* (pfsense start up for further installation/configuration)


<img width="1280" alt="Screenshot 2024-05-24 at 17 58 08" src="https://github.com/USENEDEM/Network-Endpoint-Security-applications-installations./assets/169564406/807dc8a0-07e1-4c7e-b753-079a0a88be8a">

*Ref 5.* (installation/configuration running)

3. N/B~ i removed the *Iso* file immediately after installation before rebooting the machine to avoid restarting the installation process from scratch.


<img width="1280" alt="Screenshot 2024-05-26 at 23 22 40" src="https://github.com/USENEDEM/Network-Endpoint-Security-applications-installations./assets/169564406/739fe1d8-5ffe-47ee-a55b-e68e2b965c79">


*Ref 6* (Pf sense shell interface running after successfull installation)

4. I set up my kali linux on the same home network as *pfsense* and accessed the *pfsense* graphical interface using my browser and the home *ip address* of pfsense. 

 
<img width="1280" alt="Screenshot 2024-05-26 at 22 49 26" src="https://github.com/USENEDEM/Network-Endpoint-Security-applications-installations./assets/169564406/4262b6aa-9ace-4475-b4a0-17866ac8d0ef">

*Ref 7.* ( *kali-linux* on the same *LAN* network address as pfsense)


### Snort
---

1. I ran the command
```zsh
sudo apt update
```
on my terminal to update my repository.
2. Ran  the command 
```zsh
sudo apt install snort
```
on my kali linux terminal to install snort.


<img width="1280" alt="Screenshot 2024-06-13 at 15 44 00" src="https://github.com/USENEDEM/Network-Endpoint-Security-applications-installations./assets/169564406/32e48e21-4f2f-4473-8a01-1ab21f14c43c">


*Ref 1.1 (Installation command)

3. I ran the command
```zsh
snort -h
```
to ensure snort was successfully installed and running on the system.


<img width="1280" alt="Screenshot 2024-06-13 at 15 53 51" src="https://github.com/USENEDEM/Network-Endpoint-Security-applications-installations./assets/169564406/66be5845-a094-462c-926a-9505f7187a4f">

*Ref. 2.2 (*snort* running)


### Protonvpn

1. Registered on the *protonvpn*  website.


<img width="1280" alt="Screenshot 2024-05-31 at 05 16 25" src="https://github.com/USENEDEM/Network-Endpoint-Security-applications-installations./assets/169564406/2ad127df-f14a-4048-96d6-6aae0c0f3c26">

*Ref 1.1.1* (Protonvpn.com homepage)

2. Navigated to downloads where i downloaded the *protonvpn* debian package.
3. Ran the command
```zsh
sudo apt-get install <proton debian package>
```
4. Checked the repo. package integrity and updated my package list .Ran the command
```zsh
sudo apt-get install protonvpn-gnome-desktop
```
to install the proton app


<img width="1280" alt="Screenshot 2024-06-04 at 03 26 27" src="https://github.com/USENEDEM/Network-Endpoint-Security-applications-installations./assets/169564406/558f3474-3ad6-4f9e-a542-1a0482efb141">


*Ref 2.2.* (*protonvpn* app startup page)


<img width="1280" alt="Screenshot 2024-06-04 at 03 31 22" src="https://github.com/USENEDEM/Network-Endpoint-Security-applications-installations./assets/169564406/de96a512-8cf2-4331-ab58-52d18c0a865a">

*Ref 2.3.* (*protonvpn* connection select page)

*Reference* [protonvpn](https://Protonvpn.com).
