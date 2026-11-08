# Networking Class 10 — ARP (Address Resolution Protocol)

## 1. Introduction

ARP networking ka ek important protocol hai. Is ka kaam IP address ko MAC address mein convert ya resolve karna hota hai.

Jab ek computer ko same local network mein kisi doosre computer ko data send karna hota hai, to usay destination ka MAC address chahiye hota hai.

ARP isi MAC address ko find karne mein help karta hai.

## 2. What is ARP?

**Definition:** ARP (Address Resolution Protocol) is a network protocol used to find the MAC address associated with a known IPv4 address on a local network.

Simple words mein:

ARP ek protocol hai jo IP address ki help se us device ka MAC address find karta hai.

### Example

Suppose:

- Computer A ka IP address: 192.168.1.10
- Computer B ka IP address: 192.168.1.20
- Computer B ka MAC address: AA:BB:CC:11:22:33

Computer A ko Computer B ko data send karna hai, lekin Computer A ke paas Computer B ka MAC address nahi hai.

ARP Computer B ka MAC address find karega.

## 3. What is an IP Address?

**Definition:** An IP address is a logical address assigned to a device on an IP network.

IP address network mein device ki logical identification ke liye use hota hai.

Example:
192.168.1.10

## 4. What is a MAC Address?

**Definition:** A MAC address is a hardware address used to identify a network interface on a local network.

MAC address network interface ki identification ke liye use hota hai.

Example:
AA:BB:CC:11:22:33

### IP Address vs MAC Address

| IP Address | MAC Address |
|---|---|
| Logical address | Hardware address |
| Network communication ke liye use hota hai | Local network par device identify karta hai |
| IPv4 example: 192.168.1.10 | Example: AA:BB:CC:11:22:33 |
| Network configuration ke through change ho sakta hai | Aam tor par network interface ka assigned address hota hai |

## 5. Why Do We Need ARP?

Network mein communication ke liye IP address aur MAC address dono important hain.

IP address destination device ko identify karne mein help karta hai, jab ke Ethernet network par frame deliver karne ke liye MAC address use hota hai.

ARP ki zaroorat is liye hoti hai:

1. Destination ka MAC address find karna.
2. Local network mein communication karna.
3. Ethernet frames ko correct device tak deliver karna.
4. IP address ko MAC address ke sath resolve karna.

## 6. How Does ARP Work?

ARP kaam karne ke liye ARP Request aur ARP Reply use karta hai.

### Step 1: ARP Request

Computer A ko Computer B ka MAC address chahiye.

Computer A local network mein broadcast message send karta hai:

"Who has IP address 192.168.1.20?"

Ye request local network ke devices tak pohanchti hai.

### Step 2: ARP Reply

Jis device ka IP address 192.168.1.20 hota hai, wo reply send karta hai:

"My MAC address is AA:BB:CC:11:22:33."

### Step 3: MAC Address Saved

Computer A received MAC address ko apni ARP cache mein save kar leta hai.

### Step 4: Data Transfer

Ab Computer A Ethernet frame bana kar Computer B ko data send kar sakta hai.

## 7. ARP Working Diagram

Computer A
IP: 192.168.1.10
       |
       | ARP Request (Broadcast)
       |
       v
   Local Network
       |
       | ARP Reply (Unicast)
       |
       v
Computer B
IP: 192.168.1.20
MAC: AA:BB:CC:11:22:33

Ab Computer A ko Computer B ka MAC address mil gaya hai.

## 8. What is ARP Request?

**Definition:** An ARP Request is a broadcast message used to ask which device has a particular IPv4 address.

ARP Request local network ke tamam devices ko send ki jati hai.

Example:

Who has 192.168.1.20?

## 9. What is ARP Reply?

**Definition:** An ARP Reply is a message that provides the MAC address associated with the requested IPv4 address.

ARP Reply usually us device ki taraf se aati hai jis ka IP address find kiya ja raha hota hai.

Example:

192.168.1.20 is at AA:BB:CC:11:22:33.

## 10. What is ARP Cache?

**Definition:** ARP Cache is a table that temporarily stores IP addresses and their corresponding MAC addresses.

ARP Cache computer ki temporary table hoti hai jahan IP aur MAC address ki mapping save hoti hai.

Is ka faida ye hai ke har dafa same MAC address find karne ke liye ARP Request send nahi karni parti.

### Example

| IP Address | MAC Address |
|---|---|
| 192.168.1.1 | 00:11:22:33:44:55 |
| 192.168.1.20 | AA:BB:CC:11:22:33 |

## 11. Types of ARP

### 1. Standard ARP

Standard ARP known IPv4 address ke corresponding MAC address find karta hai.

### 2. Gratuitous ARP

Gratuitous ARP mein device apne hi IP address ke liye ARP message send karta hai.

Is ke uses:

- Duplicate IP address detect karna.
- Network par apni IP-to-MAC mapping announce karna.
- Kuch network failover situations mein cache update karwana.

### 3. Proxy ARP

Proxy ARP mein router kisi doosre device ke IP address ke liye apne MAC address se reply kar sakta hai.

Is se different network segments ke darmiyan kuch communication possible hoti hai.

### 4. Reverse ARP (RARP)

RARP historically MAC address ki help se IP address find karne ke liye use hota tha.

Aaj kal is ka use bohat kam hai. Is ki jagah DHCP jaise protocols use hote hain.

## 12. What is ARP Broadcast?

ARP Request normally broadcast hoti hai.

Broadcast ka matlab hai ke message local network ke tamam devices ko send kiya jata hai.

Ethernet broadcast MAC address:

FF:FF:FF:FF:FF:FF

ARP Reply normally unicast hoti hai, yani sirf requesting device ko send ki jati hai.

## 13. ARP Commands in Windows

### 1. Display ARP Table

Command:

arp -a

Ye command computer ki ARP cache show karti hai.

### 2. Delete ARP Cache Entry

Command:

arp -d *

Ye command Windows mein ARP cache entries delete karne ke liye use hoti hai. Is ke liye administrator permission ki zaroorat ho sakti hai.

### 3. Add Static ARP Entry

Command:

arp -s 192.168.1.20 AA-BB-CC-11-22-33

Ye command static ARP entry add karne ke liye use hoti hai. Is ke liye administrator permission ki zaroorat ho sakti hai.

## 14. ARP in Linux

### 1. Show Neighbour Table

Command:

ip neigh

Ye command IP addresses aur un ke corresponding link-layer addresses show karti hai.

### 2. Show ARP Information

Command:

arp -n

Agar `arp` command installed ho to ye ARP table show karti hai.

### 3. Delete Neighbour Entry

Command:

sudo ip neigh del 192.168.1.20 dev eth0

Is command mein `eth0` ki jagah apne actual network interface ka naam use karein.

## 15. ARP and Router

Jab computer kisi doosre network mein data send karta hai, to wo destination device ka MAC address directly find nahi karta.

Is situation mein computer apne default gateway yani router ka MAC address find karta hai.

Example:

- Computer IP: 192.168.1.10
- Router IP: 192.168.1.1
- Destination IP: 8.8.8.8

Computer ARP ke through router ka MAC address find karega.

Phir data router ko send karega. Router packet ko next network ki taraf forward karega.

## 16. ARP Security Risks

ARP mein kuch security risks bhi hote hain.

### 1. ARP Spoofing

ARP Spoofing mein attacker fake ARP messages send karta hai aur IP address ke sath apna MAC address associate karne ki koshish karta hai.

### 2. ARP Poisoning

ARP Poisoning mein attacker devices ki ARP cache mein incorrect IP-to-MAC mapping insert karne ki koshish karta hai.

### 3. Man-in-the-Middle Attack

Agar attacker ARP Poisoning successfully perform kar le to wo do devices ke darmiyan traffic intercept kar sakta hai.

### Protection Methods

- Dynamic ARP Inspection (DAI) use karna.
- Network switches par DHCP Snooping configure karna.
- Secure network configuration rakhna.
- Static ARP entries sirf zaroorat ke mutabiq use karna.
- Network traffic monitor karna.

## 17. Difference Between ARP and DNS

| ARP | DNS |
|---|---|
| IP address se MAC address find karta hai | Domain name se IP address find karta hai |
| Local network mein use hota hai | Internet aur networks mein use hota hai |
| IPv4 ke liye use hota hai | IPv4 aur IPv6 dono ke records support karta hai |
| Example: IP to MAC | Example: google.com to IP |

## 18. Important Points

- ARP stands for Address Resolution Protocol.
- ARP IPv4 networks mein use hota hai.
- ARP IP address ko MAC address se resolve karta hai.
- ARP Request broadcast hoti hai.
- ARP Reply normally unicast hoti hai.
- ARP Cache IP aur MAC mapping store karti hai.
- ARP Spoofing ek security threat hai.
- IPv6 mein ARP use nahi hota; us ki jagah Neighbor Discovery Protocol (NDP) use hota hai.

## 19. Interview Questions

**Q1: What is ARP?**

ARP is a protocol used to find the MAC address associated with an IPv4 address on a local network.

**Q2: What is the full form of ARP?**

Address Resolution Protocol.

**Q3: What is the main purpose of ARP?**

To resolve an IPv4 address into a MAC address.

**Q4: What is an ARP Request?**

It is a broadcast message asking for the MAC address of a particular IPv4 address.

**Q5: What is an ARP Reply?**

It is a response that provides the requested MAC address.

**Q6: What is ARP Cache?**

It is a temporary table that stores IP-to-MAC address mappings.

**Q7: What is ARP Spoofing?**

It is an attack in which fake ARP messages are used to send incorrect IP-to-MAC mappings.

**Q8: Does IPv6 use ARP?**

No. IPv6 uses Neighbor Discovery Protocol (NDP).

**Q9: Which command displays the ARP table in Windows?**

arp -a

**Q10: What happens when a device sends data to another network?**

It resolves the MAC address of its default gateway and sends the Ethernet frame to the router.

## 20. Conclusion

ARP networking ka important protocol hai jo IPv4 address ko MAC address ke sath resolve karta hai.

Jab local network mein kisi device ko doosre device ka MAC address nahi pata hota, to ARP Request send ki jati hai.

Destination device ARP Reply send karta hai aur us ka MAC address ARP Cache mein save ho jata hai.

ARP local network communication mein important role play karta hai. Lekin ARP Spoofing jaise attacks se bachne ke liye network security measures bhi zaroori hain.
