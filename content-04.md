
# Networking Class 04 - Router Working, IP Allocation, Packets, IPv4 Structure

## 1. Introduction to Networking

Networking ka matlab hai do ya do se zyada computers ya devices ko connect karna taake woh data aur resources share kar saken.

Network mein computers, mobile phones, servers, switches aur routers jaisay devices use hotay hain.

### Main Topics

- Router Working
- IP Address Allocation
- DHCP
- Static and Dynamic IP Address
- Data Packets
- IPv4 Address Structure
- Network ID and Host ID
- Private and Public IP Addresses
- Default Gateway

## 2. What is a Router?

### Definition

A router is a networking device that forwards IP packets between different networks using routing information.

### Roman Urdu Explanation

Router aik networking device hai jo different networks ko connect karta hai. Ye IP address aur routing table ki madad se decide karta hai ke data packet ko kis network ya next device ki taraf bhejna hai.

### Example

Aap ka mobile Wi-Fi ke zariye home router se connected hai. Jab aap Google open karti hain, to aap ka data local network se router ke through internet ki taraf ja sakta hai.

### Functions of a Router

1. Different networks ko connect karna.
2. IP packets ko forward karna.
3. Routing table ki madad se route select karna.
4. Doosray network tak data pohanchane mein help karna.
5. Home routers mein NAT ke zariye private IP addresses ko public IP address ke sath map karna.
6. DHCP service provide karna, agar router mein DHCP enabled ho.

Note: Har router mein DHCP, Wi-Fi aur firewall ki functionality zaroori nahi hoti. Ye device aur configuration par depend karti hai.

## 3. How Does a Router Work?

Router data ko destination IP address ki bunyaad par forward karta hai.

### Step-by-Step Working

1. User apne mobile ya computer se website open karta hai.
2. Device destination server ke IP address tak data bhejne ki koshish karta hai.
3. Device check karta hai ke destination local network mein hai ya kisi doosray network mein.
4. Agar destination doosray network mein ho, to device packet ko default gateway ki taraf bhejta hai.
5. Router packet ka destination IP address check karta hai.
6. Router apni routing table ko check karta hai.
7. Router suitable route ya next hop select karta hai.
8. Packet aglay router ya destination network ki taraf forward hota hai.
9. Destination tak pohanchne ke baad data application ko deliver hota hai.

### Real-Life Example

Aap apne ghar mein Wi-Fi use kar rahi hain aur YouTube open karti hain.

- Mobile Wi-Fi ke through router se connect hota hai.
- Mobile ko local IP address milta hai.
- Mobile remote server ke IP address tak data bhejta hai.
- Router packet ko internet ki taraf forward karta hai.
- Server ka response wapas aata hai aur video load hoti hai.

## 4. What is an IP Address?

### Definition

An IP address is a logical address assigned to a network interface to identify it for communication using the Internet Protocol.

### Roman Urdu Explanation

IP address network par device ke interface ki logical addressing ke liye use hota hai. Is ki madad se IP packets ko source aur destination ke darmiyan route kiya ja sakta hai.

Aik device ke multiple network interfaces aur multiple IP addresses bhi ho sakte hain.

### Example

IPv4 address:

192.168.1.10

Is address ko IPv4 ke format mein four decimal numbers ki surat mein likha jata hai.

### Importance of IP Address

1. Network interfaces ki logical addressing.
2. Source aur destination identify karne mein help.
3. Different networks ke darmiyan routing.
4. Network communication ko possible banana.

## 5. IP Address Allocation

### Definition

IP address allocation is the process of assigning IP addresses to network interfaces so that they can communicate on an IP network.

### Roman Urdu Explanation

IP allocation ka matlab network ke devices ko IP addresses assign karna hai. IP address manually configure kiya ja sakta hai ya DHCP jaisi service automatically assign kar sakti hai.

### Common Methods of IP Allocation

- Static IP Allocation
- Dynamic IP Allocation
- DHCP Reservation

## 6. Static IP Address

### Definition

A static IP address is an IP address configured manually or reserved to remain consistent for a network interface.

### Roman Urdu Explanation

Static IP address aam tor par manually set kiya jata hai. Ye tab tak same rehta hai jab tak administrator ya network configuration isay change na kare.

### Example

Aik local network mein printer ka address manually set kiya ja sakta hai:

192.168.1.50

Is se users ko printer ka address consistently maloom rehta hai.

### Advantages

1. Servers aur printers ke liye useful ho sakta hai.
2. Address predictable rehta hai.
3. Network administration mein asani hoti hai.

### Disadvantages

1. Manual configuration ki zaroorat ho sakti hai.
2. Ghalat settings se connectivity issue ho sakta hai.
3. Duplicate IP address conflict paida kar sakta hai.

## 7. Dynamic IP Address

### Definition

A dynamic IP address is an IP address assigned automatically through a network configuration service such as DHCP.

### Roman Urdu Explanation

Dynamic IP address automatically assign hota hai. DHCP server address aur doosri network settings lease ki surat mein provide kar sakta hai.

Lease expire hone, renew hone ya network configuration change hone par address change ho sakta hai.

### Example

Jab aap apna mobile home Wi-Fi se connect karti hain, to router ka DHCP server aap ke mobile ko available address assign kar sakta hai.

Example:

192.168.1.101

### Advantages

1. Devices ko manually configure karne ki zaroorat kam hoti hai.
2. Network management asan hoti hai.
3. Available addresses ko efficiently reuse kiya ja sakta hai.

### Disadvantages

1. Address change ho sakta hai.
2. DHCP service mein issue aaye to device ko configuration milne mein problem ho sakti hai.

## 8. DHCP (Dynamic Host Configuration Protocol)

### Definition

DHCP is a network protocol that automatically provides IP configuration to clients.

### Roman Urdu Explanation

DHCP network devices ko automatically IP address aur doosri settings provide karta hai, jaise subnet mask, default gateway aur DNS server.

### DHCP Working: DORA Process

DHCP ka basic address allocation process chaar steps par mushtamil hota hai.

#### 1. Discover

Client network par DHCP server ko discover karne ke liye message send karta hai.

#### 2. Offer

DHCP server client ko available IP address aur configuration offer karta hai.

#### 3. Request

Client offered configuration ko request karta hai.

#### 4. Acknowledge

DHCP server request confirm karta hai aur lease details provide karta hai.

### Example

Aap laptop ko Wi-Fi se connect karti hain. DHCP server laptop ko IP address, subnet mask, default gateway aur DNS information provide kar sakta hai.

### Important Point

DHCP aur DNS different services hain.

- DHCP: IP configuration assign karta hai.
- DNS: Domain names ko IP addresses mein resolve karne mein help karta hai.

## 9. What is a Data Packet?

### Definition

A packet is a formatted unit of data carried by a network-layer protocol such as IP.

### Roman Urdu Explanation

Jab data aik device se doosray device tak send hota hai, to network protocols usay chhotay units mein carry kar sakte hain. IP networking mein in units ko packets kaha jata hai.

Har IP packet mein header hota hai aur us ke baad payload hota hai.

### Packet Structure

#### Header

Header mein networking information hoti hai, jaise:

- Source IP address
- Destination IP address
- TTL ya Hop Limit
- Protocol information
- Packet ko process aur forward karne ke liye doosri fields

#### Payload

Payload mein upper-layer data hota hai, jaise TCP segment, UDP datagram ya doosra protocol data.

### Example

Aap kisi website ko request bhejti hain. IP packets ke zariye request server tak ja sakti hai. Server ka response bhi packets ki surat mein wapas aa sakta hai.

### Important Point

IP packets zaroori nahi ke hamesha aik hi route se travel karein. Network routing ke mutabiq different packets ke routes different ho sakte hain.

## 10. Packet vs Frame

### Packet

Packet network layer, yani IP, se related data unit hai.

### Frame

Frame data-link layer par data carry karta hai, jaise Ethernet ya Wi-Fi.

### Difference

- Packet: Network layer par addressing aur routing.
- Frame: Local link par data transfer.
- Router: Aam tor par incoming frame ko process karta hai aur packet ko outgoing interface ke liye naye frame mein encapsulate karta hai.

## 11. IPv4 Structure

### Definition

IPv4 stands for Internet Protocol version 4. It uses a 32-bit address to identify network interfaces for IP communication.

### Roman Urdu Explanation

IPv4 addressing system 32 bits par mushtamil hota hai. Isay aam tor par four decimal numbers mein likha jata hai jinhein octets kehte hain.

Har octet ki value 0 se 255 tak ho sakti hai.

### Example

192.168.1.10

Is address ke four octets hain:

- First Octet: 192
- Second Octet: 168
- Third Octet: 1
- Fourth Octet: 10

Har octet 8 bits ka hota hai.

8 + 8 + 8 + 8 = 32 bits

### IPv4 Binary Structure

Example:

192.168.1.10

Binary representation:

11000000.10101000.00000001.00001010

Har group mein 8 binary bits hain.

### Total IPv4 Address Space

IPv4 address length 32 bits hai, is liye total possible bit patterns:

2^32 = 4,294,967,296

Lekin in tamam addresses ko ordinary public host addresses ke tor par use nahi kiya ja sakta. Kuch ranges special purposes ke liye reserved hain.

## 12. Network ID and Host ID

### Network ID

Network portion IP address ke us hissa ko kehte hain jo network identify karta hai.

### Host ID

Host portion IP address ke us hissa ko kehte hain jo us network ke andar interface identify karta hai.

### Example

IP address:

192.168.1.10/24

Subnet mask:

255.255.255.0

Is example mein:

- Network portion: 192.168.1
- Host portion: 10

Yahan `/24` ka matlab hai ke pehle 24 bits network prefix ka hissa hain aur baqi 8 bits host portion ke liye hain.

Network address:

192.168.1.0

Broadcast address:

192.168.1.255

Aam tor par usable host range:

192.168.1.1 - 192.168.1.254

Ye example aik ordinary IPv4 /24 subnet ko represent karta hai.

## 13. Subnet Mask and CIDR

### Definition

A subnet mask identifies which bits of an IPv4 address belong to the network prefix and which bits belong to the host portion.

### Roman Urdu Explanation

Subnet mask ki madad se device ya router samajhta hai ke IP address ka kaunsa hissa network ko identify karta hai.

### Example

IP address:

192.168.1.10

Subnet mask:

255.255.255.0

CIDR notation:

192.168.1.10/24

`/24` ka matlab hai ke network prefix ke pehle 24 bits hain.

### CIDR Examples

- /8 = 255.0.0.0
- /16 = 255.255.0.0
- /24 = 255.255.255.0
- /25 = 255.255.255.128
- /26 = 255.255.255.192

CIDR notation network prefix ki length show karti hai.

## 14. Public IP Address

### Definition

A public IP address is an address that is globally routable on the public Internet, subject to routing policies and special-purpose reservations.

### Roman Urdu Explanation

Public IP address internet par publicly routable communication ke liye use hota hai. Internet Service Provider (ISP) aap ke router ya network ko public IPv4 address provide kar sakta hai.

### Example

Home router ka internet-facing interface public IPv4 address use kar sakta hai.

### Uses

1. Internet par reachable services.
2. Public servers aur websites.
3. Networks ke darmiyan internet communication.

Note: Public IP hona is baat ki guarantee nahi ke device directly accessible bhi ho. Firewall, NAT aur routing rules access ko affect kar sakte hain.

## 15. Private IP Address

### Definition

A private IPv4 address is an address reserved for use inside private networks and is not globally routed across the public Internet.

### Roman Urdu Explanation

Private IP addresses gharon, offices, schools aur organizations ke local networks mein use hotay hain.

### Private IPv4 Ranges

- 10.0.0.0/8
- 172.16.0.0/12
- 192.168.0.0/16

### Examples

- 10.0.0.5
- 172.16.1.10
- 192.168.1.20

### Important Point

Private IP addresses ko public Internet par directly route nahi kiya jata. Internet access ke liye aam tor par NAT ya koi doosra suitable network arrangement use hota hai.

## 16. NAT (Network Address Translation)

### Definition

Network Address Translation (NAT) changes IP address information in packet headers as packets pass through a network device.

### Roman Urdu Explanation

Home routers mein NAT aksar multiple private network devices ko aik public IPv4 address ke zariye internet communication karne deta hai.

### Example

Local devices:

- Mobile: 192.168.1.10
- Laptop: 192.168.1.11
- Tablet: 192.168.1.12

Router in devices ki internet-bound connections ko apne public address ke zariye translate kar sakta hai. Aksar home routers is kaam ke liye port translation bhi use karte hain.

### Benefits

1. Public IPv4 addresses ko conserve karne mein help.
2. Multiple private devices ko internet access dena.
3. Private aur external network addressing ke darmiyan translation.

Note: NAT firewall ka replacement nahi hai aur na hi har type ka NAT aik jaisa hota hai.

## 17. Default Gateway

### Definition

A default gateway is the next-hop router used to forward packets when no more specific route matches the destination.

### Roman Urdu Explanation

Default gateway aam tor par local network ka router hota hai. Jab computer ko kisi doosray network par data send karna hota hai aur destination local subnet mein nahi hota, to packet default gateway ko bheja ja sakta hai.

### Example

Computer IP:

192.168.1.10

Subnet mask:

255.255.255.0

Default gateway:

192.168.1.1

Agar computer kisi remote website tak data bhejna chahe, to aam tor par packet router `192.168.1.1` ki taraf bhejega.

## 18. ARP and MAC Address

### ARP Definition

Address Resolution Protocol (ARP) is used on IPv4 local networks to resolve an IPv4 address to a link-layer address, such as an Ethernet MAC address.

### Roman Urdu Explanation

Jab computer ko local Ethernet network par kisi IPv4 address tak frame bhejna hota hai, to usay destination interface ka MAC address maloom karna par sakta hai.

ARP is mapping ko discover karne mein help karta hai.

### Example

Agar computer ka default gateway `192.168.1.1` hai, to computer local network par gateway ka MAC address discover kar sakta hai.

### Important Difference

- IP Address: Network-layer logical address.
- MAC Address: Link-layer address, jo local network communication mein use hota hai.
- ARP: IPv4 address se local link-layer address resolve karne ka protocol.

Agar destination remote network par ho, to local computer aam tor par remote server ka MAC address discover nahi karta; woh default gateway ka MAC address use karta hai.

## 19. Router vs Switch

### Router

- Different IP networks ke darmiyan packets forward karta hai.
- Routing table use karta hai.
- Network layer par kaam karta hai.

### Switch

- Local network mein Ethernet frames forward karta hai.
- Aam tor par MAC address table use karta hai.
- Traditional Layer 2 switch data-link layer par kaam karta hai.

Note: Layer 3 switches routing bhi perform kar sakte hain.

## 20. Practical Lab

### Step 1: Windows IP Configuration

Command Prompt open karein aur type karein:

```cmd
ipconfig
```

Ye IP address, subnet mask aur default gateway ki information show kar sakta hai.

### Step 2: Detailed IP Configuration

```cmd
ipconfig /all
```

Ye network adapter ki detailed configuration display karta hai.

### Step 3: Linux IP Address Check

```bash
ip addr
```

Ye Linux network interfaces aur un ke assigned addresses show karta hai.

### Step 4: Linux Routing Table Check

```bash
ip route
```

Ye routing table aur default route ki information show karta hai.

### Step 5: Gateway Connectivity Test

Windows ya Linux par:

```bash
ping 192.168.1.1
```

Apne actual default gateway ke address se `192.168.1.1` replace karein.

Note: Ping ka response na aana zaroori nahi ke router band hai. Firewall ya network policy ICMP ko block kar sakti hai.

## 21. Quick Revision

- Router: Different networks ke darmiyan IP packets forward karta hai.
- IP Address: Network interface ki logical addressing ke liye use hota hai.
- Static IP: Manually configure ya consistently reserve kiya gaya address.
- Dynamic IP: DHCP jaisi service se automatically assign hone wala address.
- DHCP: Network configuration provide karta hai.
- Packet: Network layer par data ki formatted unit.
- IPv4: 32-bit addressing system.
- Octet: IPv4 address ka 8-bit group.
- Subnet Mask: Network aur host portion identify karta hai.
- CIDR: Network prefix length show karta hai.
- Public IP: Public Internet par globally routable address.
- Private IP: Private networks ke liye reserved IPv4 address.
- NAT: Packet address information translate karta hai.
- Default Gateway: Doosray networks ke liye aam next-hop router.
- ARP: IPv4 address ko local link-layer address se resolve karta hai.
- MAC Address: Local link par frame delivery ke liye address.

## 22. Conclusion

Router, IP allocation, packets aur IPv4 structure networking ke basic aur important concepts hain.

Router packets ko routing table ki madad se forward karta hai. DHCP devices ko network configuration provide kar sakta hai. IPv4 32-bit addressing use karta hai, jabke subnet mask aur CIDR network prefix identify karne mein help karte hain.

In concepts ki practical practice se networking, troubleshooting aur cybersecurity ki understanding improve hoti hai.
