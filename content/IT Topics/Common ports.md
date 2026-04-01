---
title: common ports
catagories: "networking"
type: post
---

### World Wide Web Protocols

|Port|Transport Protocol|Application Protocol|Description|
|---|---|---|---|
|53|TCP, UDP|DNS|The Domain Name Service (DNS) protocol finds the IP address associated with a registered Internet domain for Web, Email, and other Internet services. It uses UDP for requests and information transfer between DNS servers. TCP will be used for DNS responses if req1uired.|
|80|TCP|HTTP|Hypertext Transfer Protocol (HTTP) provides a set of rules for exchanging text, graphic images, sound, video, and other multimedia files on the World Wide Web|
|443|TCP, UDP|HTTPS|The browser uses encryption and authenticates your connection with webserver.|

### Email and Identity Management Protocols

|Port|Transport Protocol|Application Protocol|Description|
|---|---|---|---|
|25|TCP|SMTP|Simple Mail Transfer Protocol is used to send email from clients to an email server. It may also be used to relay email messages from source to destination email servers.|
|110|TCP|POP3|Post Office Protocol 3 is used by email clients to retrieve messages from an email server.|
|143|TCP|IMAP|Internet Message Access Protocol is used to retrieve email messages from a server. It is more advanced than POP3 and offers a number of advantages.|
|389|TCP, UDP|LDAP1|Lightweight Directory Access Protocol is used to maintain user identity directory information that can be shared across networks and systems. It can be used to manage information about users and network resources. It can be used to authenticate users on multiple computers.2|

---

### File Transport and Management Protocols

|Port|Transport Protocol|Application Protocol|Description|
|---|---|---|---|
|20|TCP|FTP|File transfer protocol. Used to transfer files between computers. Considered insecure, SSH file transfer protocol (SFTP, TCP port 22) should be used.|
|21|TCP|FTP|FTP uses TCP port 21 to establish a connection between the client and FTP server. In order to start a data transfer session.|
|69|UDP|TFTP|Trivial File Transfer Protocol utilizes less overhead than FTP.|
|445|TCP|SMB/CIFS|Server Message Block or Common Internet File System allow for sharing of files, printers, and other resources between nodes on a network.|
|548|TCP, UDP|AFP|Apple Filing Protocol is a proprietary protocol developed by Apple to enable file services for macOS and classic Mac OS.|

### Remote Access Protocols

|Port|Transport Protocol|Application Protocol|Description|
|---|---|---|---|
|22|TCP|SSH|**Secure Shell** or **Secure Socket Shell** provides a strong authentication and encrypted data transport between a client and remote computer. Like Telnet, it provides a command line on the remote computer.|
|23|TCP|Telnet|**Telnet** is an insecure remote access protocol that provides a command line on a remote computer. SSH is preferred for security reasons.|
|3389|TCP, UDP|RDP|**Remote desktop protocol** was developed by Microsoft to provide remote access to the graphical desktop of a remote machine. It is useful for tech support situations, however it should be used with caution because it provides a remote user with complete control of the destination computer.|

---

### Network Operations Protocols

|Port|Transport Protocol|Application Protocol|Description|
|---|---|---|---|
|67/68|UDP|DHCP|**Dynamic Host Configuration Protocol** automatically provides IP addresses to network hosts and provides a way to manage those addresses. The DHCP server uses UDP port 67 and the client host uses UDP port 68.|
|137–139|UDP, TCP|NetBIOS (NetBT)1|**NetBIOS over TCP/IP** provides a system through which older computer applications can communicate over large TCP/IP networks. Different NetBT functions use different protocols and ports in t2his range.|
|161/162|UDP|SNMP|**Simple Network Management Protocol** enables network administrators to monitor network operations from centralized monitoring stations.|
|427|UDP, TCP|SLP|**Service Location Protocol** allows computers and other devices to locate services on a LAN without previous configuration. Usually uses UDP, but can use TCP.|
|445|UDP, TCP|SMB|**Server Message Block (SMB)** is a client/server file sharing protocol that describes the structure of shared network resources, such as directories, files, printers, and serial ports. SMB file-sharing and print services have become the mainstay of Microsoft networking.|

### **Application Protocols in Port Number Order**

| Port Number | Protocol | Application   |
| ----------- | -------- | ------------- |
| 20          | TCP      | FTP (data)    |
| 21          | TCP      | FTP (control) |
| 22          | TCP      | SSH           |
| 23          | TCP      | Telnet        |
| 25          | TCP      | SMTP          |
| 53          | TCP, UDP | DNS           |
| 67          | UDP      | DHCP (server) |
| 68          | UDP      | DHCP (client) |
| 69          | UDP      | TFTP          |
| 80          | TCP      | HTTP          |
| 110         | TCP      | POP3          |
| 137-139     | TCP, UDP | NetBIOS NetBT |
| 143         | TCP      | IMAP          |
| 161/162     | UDP      | SNMP          |
| 389         | TCP, UDP | LDAP          |
| 427         | TCP, UDP | SLP           |
| 443         | TCP, UDP | HTTPS         |
| 445         | TCP      | SMB/CIFS      |
| 548         | TCP      | AFP           |
| 3389        | TCP, UDP | RDP           |






