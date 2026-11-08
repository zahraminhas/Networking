# Networking Class 07 — TCP/IP Model (Detail)

## 1. Introduction to TCP/IP Model

TCP/IP stands for Transmission Control Protocol / Internet Protocol.

TCP/IP Model aik networking model hai jo explain karta hai ke computers aur devices internet ya network ke through kis tarah communicate karte hain.

Ye model data ko aik device se doosray device tak send aur receive karne mein help karta hai.

TCP/IP Model internet communication ka basic foundation hai.

## 2. Layers of TCP/IP Model

TCP/IP Model mein 4 main layers hoti hain.

1. Application Layer
2. Transport Layer
3. Internet Layer
4. Network Access Layer

Har layer ka apna specific function hota hai.

## 3. Layer 4 — Application Layer

Application Layer TCP/IP Model ki top layer hai.

Ye users aur applications ko network services provide karti hai.

Is layer mein OSI Model ki Application, Presentation aur Session layers ke functions combine hote hain.

### Functions

- Web browsing
- Email communication
- File transfer
- Data formatting
- Application communication

### Protocols

- HTTP (Hypertext Transfer Protocol)
- HTTPS (Hypertext Transfer Protocol Secure)
- FTP (File Transfer Protocol)
- SMTP (Simple Mail Transfer Protocol)
- DNS (Domain Name System)
- DHCP (Dynamic Host Configuration Protocol)
- SSH (Secure Shell)

### Real-Life Example

Jab hum Google Chrome open karke kisi website ko visit karte hain to Application Layer network communication mein help karti hai.

## 4. Layer 3 — Transport Layer

Transport Layer aik device se doosray device tak data delivery manage karti hai.

Ye Application Layer se data receive karti hai aur usay smaller segments mein divide kar sakti hai.

### Functions

- End-to-End Communication
- Data Segmentation
- Flow Control
- Error Recovery
- Port Number Management
- Reliable Data Delivery

### Main Protocols

**1. TCP (Transmission Control Protocol)**

TCP aik connection-oriented aur reliable protocol hai.

Ye ensure karta hai ke data correct order mein destination tak pohanchay.

TCP missing data ko retransmit bhi kar sakta hai.

### TCP Features

- Reliable communication
- Connection establishment
- Error recovery
- Data sequencing
- Acknowledgment

**Example:** Website access, email aur file transfer.

**2. UDP (User Datagram Protocol)**

UDP aik connectionless protocol hai.

Ye data ko quickly send karta hai lekin delivery aur correct order ki guarantee nahi deta.

### UDP Features

- Fast communication
- Low overhead
- No connection establishment
- No guaranteed delivery
- No guaranteed ordering

**Example:** Online gaming, live streaming aur video calls.

## 5. Layer 2 — Internet Layer

Internet Layer TCP/IP Model ki important layer hai.

Ye data packets ko source se destination tak different networks ke through transfer karne mein help karti hai.

Ye logical addressing aur routing perform karti hai.

### Functions

- IP Addressing
- Routing
- Packet Forwarding
- Logical Addressing
- Network-to-Network Communication

### Protocols

**1. IP (Internet Protocol)**

IP addresses ki madad se devices ko identify karta hai aur packets ko destination tak route karne mein help karta hai.

**2. ICMP (Internet Control Message Protocol)**

ICMP network errors aur diagnostic information report karne ke liye use hota hai.

**Example:** Ping command.

**3. IPv4**

IPv4 aik 32-bit IP addressing system hai.

Example: 192.168.1.1

**4. IPv6**

IPv6 aik 128-bit IP addressing system hai.

Example: 2001:db8::1

### Device

Router.

### Real-Life Example

Jab hum kisi website ko open karte hain to Internet Layer IP addressing aur routing ke through packets ko destination tak pohanchane mein help karti hai.

## 6. Layer 1 — Network Access Layer

Network Access Layer TCP/IP Model ki lowest layer hai.

Ye device ko physical network ke through connect karne aur data transmit karne mein help karti hai.

Is layer mein OSI Model ki Data Link aur Physical layers ke functions combine hote hain.

### Functions

- Physical Data Transmission
- MAC Addressing
- Frame Formation
- Error Detection
- Network Media Access

### Technologies

- Ethernet
- Wi-Fi
- Fiber Optic
- LAN

### Devices

- Switch
- Hub
- Network Interface Card (NIC)

### Real-Life Example

Jab computer Ethernet cable ya Wi-Fi ke through network se connect hota hai to Network Access Layer communication mein help karti hai.

## 7. TCP/IP Model Summary

| Layer | Main Function | Examples |
|---|---|---|
| Application | Network Services | HTTP, FTP, DNS |
| Transport | Data Delivery | TCP, UDP |
| Internet | IP Addressing and Routing | IP, ICMP |
| Network Access | Physical Network Communication | Ethernet, Wi-Fi |

## 8. Difference Between TCP and UDP

| TCP | UDP |
|---|---|
| Connection-oriented | Connectionless |
| Reliable | No delivery guarantee |
| Slower in comparison | Generally faster |
| Uses acknowledgments | No delivery acknowledgments |
| Maintains data order | No guaranteed ordering |
| Used for file transfer | Used for live streaming |

## 9. Difference Between OSI and TCP/IP Model

| OSI Model | TCP/IP Model |
|---|---|
| Has 7 layers | Has 4 layers |
| Reference model | Protocol suite and model |
| Developed by ISO | Developed through DARPA/DoD research |
| Application, Presentation and Session are separate | Combined into Application Layer |
| Physical and Data Link are separate | Combined into Network Access Layer |
| Mainly used for learning and troubleshooting | Widely used in real-world networking |

## 10. OSI and TCP/IP Layer Mapping

| OSI Model | TCP/IP Model |
|---|---|
| Application | Application |
| Presentation | Application |
| Session | Application |
| Transport | Transport |
| Network | Internet |
| Data Link | Network Access |
| Physical | Network Access |

## 11. How TCP/IP Model Works

Jab hum internet par kisi website ko open karte hain to TCP/IP Model different steps mein kaam karta hai.

### Step 1 — Application Layer

User browser mein website ka address enter karta hai.

Application Layer HTTP ya HTTPS jaise protocols use karti hai.

### Step 2 — Transport Layer

Transport Layer TCP ya UDP ke through data delivery manage karti hai.

TCP connection-oriented communication mein three-way handshake use karta hai.

### Step 3 — Internet Layer

Internet Layer source aur destination IP addresses use karti hai.

Ye packets ko correct destination ki taraf route karne mein help karti hai.

### Step 4 — Network Access Layer

Data frames aur physical signals ke through network par transmit hota hai.

### Step 5 — Receiving Device

Destination device data receive karta hai aur layers reverse order mein process karti hain.

Is process ko Decapsulation kehte hain.

## 12. Encapsulation in TCP/IP Model

Encapsulation ka matlab hai data ke sath additional information add karna jab data Application Layer se Network Access Layer ki taraf move karta hai.

### Encapsulation Process

1. Application Layer — Data
2. Transport Layer — Segment / Datagram
3. Internet Layer — Packet
4. Network Access Layer — Frame
5. Physical Transmission — Bits

## 13. Decapsulation in TCP/IP Model

Decapsulation encapsulation ka opposite process hai.

Jab destination device data receive karta hai to har layer apni required information process karti hai.

Aakhir mein original data Application Layer tak pohanch jata hai.

## 14. Important Port Numbers

| Protocol | Port Number |
|---|---|
| HTTP | 80 |
| HTTPS | 443 |
| FTP | 20, 21 |
| SSH | 22 |
| DNS | 53 |
| DHCP | 67, 68 |
| SMTP | 25 |
| POP3 | 110 |
| IMAP | 143 |

## 15. Advantages of TCP/IP Model

- Internet communication provide karta hai.
- Different devices ko connect karta hai.
- Reliable communication support karta hai.
- Different network technologies support karta hai.
- Routing aur addressing mein help karta hai.
- Large networks mein communication possible banata hai.

## 16. Important Interview Questions

**Q1: What is the full form of TCP/IP?**

Answer: Transmission Control Protocol / Internet Protocol.

**Q2: How many layers are in TCP/IP Model?**

Answer: Four Layers.

**Q3: What are the four layers of TCP/IP Model?**

Answer:
1. Application Layer
2. Transport Layer
3. Internet Layer
4. Network Access Layer

**Q4: Which layer uses TCP and UDP?**

Answer: Transport Layer.

**Q5: Which layer handles IP addressing?**

Answer: Internet Layer.

**Q6: Which layer uses HTTP and HTTPS?**

Answer: Application Layer.

**Q7: What is the difference between TCP and UDP?**

Answer: TCP provides reliable data delivery while UDP provides faster communication without guaranteed delivery.

**Q8: What is the full form of IP?**

Answer: Internet Protocol.

**Q9: What is the full form of DNS?**

Answer: Domain Name System.

**Q10: What is the full form of HTTP?**

Answer: Hypertext Transfer Protocol.

**Q11: Which protocol is used for secure remote login?**

Answer: SSH.

**Q12: What is the function of Internet Layer?**

Answer: IP addressing and routing.

## 17. Conclusion

TCP/IP Model computer networking ka aik important model hai.

Is model mein four main layers hoti hain aur har layer network communication mein apna specific role perform karti hai.

TCP/IP Model internet communication ki foundation hai.

OSI Model aur TCP/IP Model ko understand karna networking, system administration aur cybersecurity students ke liye bohat important hai.

**End of Networking Class 07**
