# Networking Class 06 — OSI Model (7 Layers)

## 1. Introduction to OSI Model

OSI stands for Open Systems Interconnection.

OSI Model aik networking model hai jo explain karta hai ke aik computer se doosray computer tak data kis tarah travel karta hai.

Is model mein network communication ko 7 different layers mein divide kiya gaya hai. Har layer ka apna specific function hota hai.

## 2. Seven Layers of OSI Model

1. Application Layer
2. Presentation Layer
3. Session Layer
4. Transport Layer
5. Network Layer
6. Data Link Layer
7. Physical Layer

## 3. Layer 7 — Application Layer

Application Layer OSI Model ki sab se upper layer hai. Ye users aur applications ko network services provide karti hai.

**Functions:**
- Web browsing
- Email communication
- File transfer
- Network services

**Protocols:** HTTP, HTTPS, FTP, SMTP, DNS.

**Example:** Jab hum Google Chrome mein website open karte hain to Application Layer network services provide karti hai.

## 4. Layer 6 — Presentation Layer

Presentation Layer data ko suitable format mein convert karti hai taake receiving computer usay samajh sake.

**Functions:**
- Data Encryption
- Data Decryption
- Data Compression
- Data Formatting

**Examples:** JPEG, PNG, ASCII.

## 5. Layer 5 — Session Layer

Session Layer do devices ke darmiyan communication session ko establish, manage aur terminate karti hai.

**Functions:**
- Session Establishment
- Session Maintenance
- Session Termination

**Example:** Online application mein login karne ke baad communication session maintain hota hai.

## 6. Layer 4 — Transport Layer

Transport Layer aik device se doosray device tak data delivery manage karti hai.

**Functions:**
- Data Segmentation
- End-to-End Communication
- Flow Control
- Error Recovery

**TCP (Transmission Control Protocol):**

TCP reliable protocol hai. Ye data ko correct order mein deliver karne aur missing data ko retransmit karne mein help karta hai.

**UDP (User Datagram Protocol):**

UDP fast communication provide karta hai lekin data delivery ki guarantee nahi deta.

**Examples:** Video calls, online gaming.

## 7. Layer 3 — Network Layer

Network Layer data ko aik network se doosray network tak transfer karne ke liye routing perform karti hai.

**Functions:**
- IP Addressing
- Routing
- Packet Forwarding
- Best Path Selection

**Protocol:** IP (Internet Protocol).

**Device:** Router.

## 8. Layer 2 — Data Link Layer

Data Link Layer same local network mein devices ke darmiyan data transfer karne mein help karti hai.

**Functions:**
- Framing
- MAC Addressing
- Error Detection
- Media Access Control

**Devices:** Switch and Bridge.

## 9. Layer 1 — Physical Layer

Physical Layer OSI Model ki sab se lower layer hai.

Ye raw bits (0s and 1s) ko physical medium ke through transfer karti hai.

**Functions:**
- Bit Transmission
- Electrical Signals
- Optical Signals
- Wireless Signals
- Cables and Connectors

**Examples:**
- Ethernet Cable
- Fiber Optic Cable
- Wireless Signals

**Devices:** Hub and Repeater.

## 10. OSI Model Data Units

| Layer | Data Unit |
|---|---|
| Application | Data |
| Presentation | Data |
| Session | Data |
| Transport | Segment / Datagram |
| Network | Packet |
| Data Link | Frame |
| Physical | Bits |

## 11. Encapsulation

Encapsulation ka matlab hai data ke sath additional information add karna jab data upper layers se lower layers ki taraf travel karta hai.

**Process:**

1. Application Layer — Data
2. Transport Layer — Segment
3. Network Layer — Packet
4. Data Link Layer — Frame
5. Physical Layer — Bits

## 12. Decapsulation

Decapsulation encapsulation ka opposite process hai.

Is process mein receiving device par data ke headers aur trailers remove kiye jate hain.

Data lower layers se upper layers ki taraf move karta hai aur original data application tak pohanchta hai.

## 13. Advantages of OSI Model

- Network communication samajhna easy banata hai.
- Network troubleshooting mein help karta hai.
- Networking ko different layers mein divide karta hai.
- Protocols ko understand karna easy banata hai.
- Network standardization mein help karta hai.

## 14. Real-Life Example of OSI Model

Jab hum WhatsApp par message send karte hain:

1. Application Layer message ko handle karti hai.
2. Presentation Layer data formatting aur encryption jaise functions se related hoti hai.
3. Session Layer communication session manage karti hai.
4. Transport Layer data delivery manage karti hai.
5. Network Layer IP addressing aur routing handle karti hai.
6. Data Link Layer frames aur MAC addressing handle karti hai.
7. Physical Layer signals ke through bits transmit karti hai.

## 15. Important Interview Questions

**Q1: What is the full form of OSI?**

Answer: Open Systems Interconnection.

**Q2: How many layers are in the OSI Model?**

Answer: Seven Layers.

**Q3: Which is the top layer?**

Answer: Application Layer.

**Q4: Which is the bottom layer?**

Answer: Physical Layer.

**Q5: Which layer uses IP addresses?**

Answer: Network Layer.

**Q6: Which layer uses MAC addresses?**

Answer: Data Link Layer.

**Q7: Which layer uses TCP and UDP?**

Answer: Transport Layer.

**Q8: Which device works at Network Layer?**

Answer: Router.

**Q9: Which device commonly works at Data Link Layer?**

Answer: Switch.

**Q10: Which layer transfers bits?**

Answer: Physical Layer.

## 16. Conclusion

OSI Model networking ka aik important concept hai. Is model mein 7 layers hoti hain aur har layer network communication mein apna specific role perform karti hai.

OSI Model ko understand karne se networking aur troubleshooting seekhna easy ho jata hai.

**End of Networking Class 06**
