---
title: Cyber attacks | Malware, Ransomeware, DOS
type: posts
---

These are the types of cyber attacks and tactics i learned during my course and put the most interesting ones here.

# Malware

Cybercriminals use many different types of malicious software, or malware, to carry out attacks.

| Viruses A virus is a type of computer program that, when executed, replicates and attaches itself to other files, such as legitimate programs, by inserting its own code into the file. Some viruses are harmless yet others can be destructive, such as those that modify or delete data. Most viruses require end-user interaction to initiate activation, and can be written to act on a specific date or time. Viruses can be spread through removable media such as USB flash drives, internet downloads, and email attachments. The simple act of opening a file or executing an infected program can trigger a virus. Once a virus is active, it will usually infect other programs on the computer or other computers on the network. Viruses mutate to avoid detection. For example, the Melissa virus was released in 1999 and spread via email, affecting tens of thousands of users and causing an estimated $1.2 billion in damage.  | Worms A worm is a malicious software program that replicates by independently exploiting vulnerabilities in networks. Unlike a virus, which requires a host program to run, worms can run by themselves. Other than the initial infection of the host, they do not require user participation and can spread very quickly over the network, usually slowing it down. Worms share similar patterns: they exploit system vulnerabilities, they have a way to propagate themselves, and they all contain malicious code (payload) that causes damage to computer systems or networks. Worms are responsible for some of the most devastating attacks on the internet. In 2001, the Code Red worm infected over 300,000 servers in just 19 hours.  | Trojan horse A Trojan horse is malware that carries out malicious operations by masking its true intent. It might appear legitimate but is, in fact, very dangerous. Trojans exploit the privileges of the user who runs them. Unlike viruses, Trojans do not self-replicate but often bind themselves to non-executable files, such as image, audio, or video files, that act as a decoy to harm the systems of unsuspecting users.  |
| :---- | :---- | :---- |

# Logic Bombs

A logic bomb is a malicious program that waits for a trigger, such as a specified date or database entry, to set off malicious code. Until this trigger event happens, the logic bomb will remain inactive.

Once activated, a logic bomb implements malicious code that causes harm to a computer in various ways. It can sabotage database records, erase files, and attack operating systems or applications. 

Cybersecurity specialists have recently discovered logic bombs that attack and destroy the hardware components in a device or server, including cooling fans, central processing units (CPU), memory, hard drives, and power supplies

# Ransomware

This malware is designed to hold a computer system or the data it contains captive until a payment is made. Ransomware usually works by encrypting your data so that you cannot access it.

It is paid usually with Crypto such as Bitcoin and ETH.

# Denial of Service Attacks

Denial of service (DoS) attacks are a type of network attack that is relatively simple to conduct, even for an unskilled attacker. These attacks are a major risk as they usually result in some sort of interruption to network services, causing a significant loss of time and money.

# 

# Domain Name System

There are many essential technical services needed for a network to operate — such as routing, addressing, and domain naming. These are prime targets for attack.

| Domain Reputation The Domain Name System (DNS) is used by DNS servers to translate a domain name, such as www.cisco.com, into a numerical IP address so that computers can understand it. If a DNS server does not know an IP address, it will ask another DNS server. An organization needs to monitor its domain reputation, including its IP address, to help protect against malicious external domains. Domain reputation is used to classify emails as spam or potential security threats. | Uniform Resource Locator (URL) Redirection A uniform resource locator (URL) is a unique identifier for finding a specific resource on the Internet. Redirecting a URL commonly happens for legitimate purposes. For example, you have logged into an eLearning portal to begin this course. If you log out of the portal and return to it another time, the portal will redirect you back to the login page.  It is this type of functionality that attackers can exploit. Instead of taking you to the eLearning login page, they can redirect you to a malicious site.  |
| :---- | :---- |
| **DNS Spoofing** DNS spoofing or DNS cache poisoning is an attack in which false data is introduced into a DNS resolver cache — the temporary database on a computer’s operating system that records recent visits to websites and other internet domains. These attacks exploit a weakness in the DNS caching software that causes DNS servers to redirect traffic for a legitimate domain to the IP address of an illicit server. | **Domain Hijacking** When an attacker wrongfully gains control of a target’s DNS information, they can make unauthorized changes to it. This is known as domain hijacking. The most common way of hijacking a domain name is to change the administrator’s contact email address through social engineering or by hacking into the administrator's email account. The administrator’s email address can be easily found via the WHOIS record for the domain, which is of public record. |

# 

# Layer 2 Attacks

the data link layer in the Open Systems Interconnection (OSI) data communication model.

This layer is used to move data across a linked physical network. IP addresses are mapped to each physical device address (also known as media access control (MAC) address) on the network, using a procedure called address resolution protocol (ARP). 

In its simplest terms, the MAC address identifies the intended receiver of an IP address sent over the network, and ARP resolves IP addresses to MAC addresses for transmitting data. 

| Spoofing  Spoofing, or poisoning, is a type of impersonation attack that takes advantage of a trusted relationship between two systems. MAC address spoofing occurs when an attacker disguises their device as a valid one on the network and can therefore bypass the authentication process.  ARP spoofing sends spoofed ARP messages across a LAN. This links an attacker’s MAC address to the IP address of an authorized device on the network. IP spoofing sends IP packets from a spoofed source address in order to disguise the packet origin. | MAC Flooding  Devices on a network are connected via a network switch by using packet switching to receive and forward data to the destination device. MAC flooding compromises the data transmitted to a device. An attacker floods the network with fake MAC addresses, compromising the security of the network switch. |
| :---- | :---- |

# Man-in-the-Middle 

A MitM attack, also known as an on-path attack, happens when a cybercriminal takes control of an intermediate device without the user's knowledge. With this level of access, an attacker can intercept, manipulate, and relay false information between the sender and the intended destination.

# Man-in-the-Mobile

Man-in-the-Mobile (MitMo)

A variation of man-in-the-middle, MitMo is a type of attack used to take control over a user's mobile device. When infected, the mobile device is instructed to exfiltrate user-sensitive information and send it to the attackers.

ZeuS is one example of a malware package with MitMo capabilities. It allows attackers to quietly capture two-step verification SMS messages sent to users.

# Zero-day Attacks

A zero-day attack, or zero-day, threat exploits software vulnerabilities before they become known or before they are disclosed by the software vendor.

A network is extremely vulnerable to attack between the time an exploit is discovered (zero hour) and the time it takes for the software vendor to develop and release a patch that fixes the vulnerability.

Defending against such fast-moving attacks requires network security professionals to adopt a more sophisticated and holistic view of any network architecture.

# Keyboard Logging

As the name suggests, keyboard logging or keylogging refers to recording or logging every key struck on a computer’s keyboard.  
They can monitor for potential personal info and passwords.

# Defending Against Attacks

Organizations can take several steps to defend against various attacks. These include the following:

* Configure firewalls to remove any packets from outside the network that have addresses indicating that they originated from inside the network.   
* Ensure patches and upgrades are current.  
* Distribute workloads across multiple server systems.  
* Network devices use Internet Control Message Protocol (ICMP) packets to send error and control messages, such as whether or not a device can communicate with another on the network. To prevent DoS and DDoS attacks, organizations can block external ICMP packets with their firewalls.

#  

# Wireless And Mobile Device Attacks

# Grayware and SMIShing

| Grayware is any unwanted application that behaves in an annoying or undesirable manner. And while grayware may not carry any recognizable malware, it may still pose a risk to the user by, for example, tracking your location or delivering unwanted advertising. Authors of grayware typically maintain legitimacy by including these ‘gray’ capabilities in the small print of the software license agreement. This factor poses a growing threat to mobile security in particular, as many smartphone users install mobile apps without really considering this small print.   | SMiShing  Fake text messages prompt you to visit a malicious website or call a fraudulent phone number, which may result in malware being downloaded onto your device or personal information being shared.  |
| :---- | :---- |

# Rogue Access Points

A rogue access point is a wireless access point installed on a secure network without explicit authorization. 

- An attacker will often use social engineering tactics to gain physical access to an organization’s network infrastructure and install the **rogue access point**.

- the access point can be set up as a MitM device to capture your login information. This works by disconnecting the rogue access point, which triggers the network to send a deauthentication frame to disassociate the access point. This process is then exploited by spoofing your MAC address and sending a deauthentication data transmission to the wireless access point.


- An **evil twin attack** describes a situation where the attacker’s access point is set up to look like a better connection option. Once you connect to the evil access point, the attacker can analyze your network traffic and execute MitM attacks.


# Radio frequency Jamming

Wireless signals are susceptible to electromagnetic interference (EMI), radio frequency interference (RFI), and even lightning strikes or noise from fluorescent lights.

Attackers can take advantage of this fact by deliberately jamming the transmission of a radio or satellite station to prevent a wireless signal from reaching the receiving station.

# Bluejacking and Bluesnarfing

Due to the limited range of Bluetooth, an attacker must be within range of their target. Here are some ways that they can exploit a target's device without their knowledge.  
