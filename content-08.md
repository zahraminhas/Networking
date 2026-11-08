# Networking Class 08 — TCP, UDP aur Handshake (Poori Detail)

## 1. Introduction to TCP and UDP

TCP aur UDP dono Transport Layer ke protocols hain.

Ye protocols aik computer se doosray computer tak data transfer karne mein help karte hain.

TCP reliable communication provide karta hai jabke UDP fast communication provide karta hai.

Dono protocols TCP/IP Model ki Transport Layer par kaam karte hain.

## 2. What is TCP?

TCP stands for Transmission Control Protocol.

TCP aik connection-oriented protocol hai jo reliable data transmission provide karta hai.

Iska matlab hai ke TCP data ko correct order mein destination tak pohanchane ki koshish karta hai.

Agar data ka koi part missing ho jaye to TCP usay dobara send kar sakta hai.

### Functions of TCP

- Reliable Data Transmission
- Error Detection
- Data Segmentation
- Flow Control
- Congestion Control
- Data Sequencing
- Acknowledgment
- Retransmission

### Features of TCP

1. Connection-oriented protocol.
2. Reliable data delivery.
3. Maintains data order.
4. Uses acknowledgment.
5. Supports retransmission.
6. Provides flow control.
7. Uses congestion control.

### TCP Examples

- Website browsing
- Email communication
- File downloading
- Secure file transfer
- Remote login

## 3. How TCP Works

TCP communication establish karne ke liye Three-Way Handshake use karta hai.

Is process mein client aur server aik doosray ke sath connection establish karte hain.

### TCP Communication Steps

1. Client server ko connection request send karta hai.
2. Server request receive karke response send karta hai.
3. Client response receive karke acknowledgment send karta hai.
4. Connection establish ho jata hai.
5. Ab dono devices data transfer kar sakte hain.

## 4. What is UDP?

UDP stands for User Datagram Protocol.

UDP aik connectionless protocol hai jo data ko quickly send karta hai.

Is protocol mein connection establish karne ke liye handshake ki zaroorat nahi hoti.

UDP data delivery, retransmission aur correct order ki guarantee nahi deta.

### Functions of UDP

- Fast Data Transmission
- Low Communication Overhead
- Datagram Delivery
- Port Number Management

### Features of UDP

1. Connectionless protocol.
2. Fast communication.
3. Low overhead.
4. No delivery guarantee.
5. No guaranteed data ordering.
6. No built-in retransmission.
7. No built-in flow control.

### UDP Examples

- Online Gaming
- Live Video Streaming
- Voice Calls
- DNS Queries
- Video Conferencing

## 5. Difference Between TCP and UDP

| TCP | UDP |
|---|---|
| Connection-oriented | Connectionless |
| Reliable delivery | No delivery guarantee |
| Uses acknowledgment | No delivery acknowledgment |
| Retransmits missing data | No built-in retransmission |
| Maintains data order | No guaranteed order |
| More overhead | Less overhead |
| Uses flow control | No built-in flow control |
| Uses congestion control | No built-in congestion control |
| Generally slower | Generally faster |
| Used for file transfer | Used for live streaming |

## 6. What is Handshake?

Handshake aik process hai jisme do devices communication start karne se pehle information exchange karte hain.

TCP connection establish karne ke liye Three-Way Handshake use karta hai.

Handshake ka main purpose client aur server ke darmiyan connection establish karna hai.

## 7. TCP Three-Way Handshake

TCP Three-Way Handshake mein three steps hote hain.

### Step 1 — SYN (Synchronize)

Client server ko SYN packet send karta hai.

Is packet mein client apna initial sequence number send karta hai.

Iska purpose connection establish karne ki request karna hai.

### Step 2 — SYN-ACK (Synchronize Acknowledgment)

Server client ki SYN request receive karta hai.

Server apna SYN aur ACK packet send karta hai.

Iska matlab hai ke server connection ke liye ready hai.

### Step 3 — ACK (Acknowledgment)

Client server ka response receive karta hai.

Client ACK packet send karta hai.

Ab TCP connection successfully establish ho jata hai.

### Three-Way Handshake Diagram

Client                         Server

   |                              |
   | -------- SYN -------------> |
   |                              |
   | <------ SYN-ACK ----------- |
   |                              |
   | -------- ACK -------------> |
   |                              |
   |      Connection Established |
   |                              |

## 8. Important TCP Flags

TCP flags connection ko establish, manage aur terminate karne mein help karte hain.

### Main TCP Flags

**1. SYN (Synchronize)**

Connection establish karne ke liye use hota hai.

**2. ACK (Acknowledgment)**

Received data ya connection request ko acknowledge karta hai.

**3. FIN (Finish)**

Connection ko normally close karne ke liye use hota hai.

**4. RST (Reset)**

Connection ko immediately reset ya terminate karne ke liye use hota hai.

**5. PSH (Push)**

Data ko receiving application tak promptly deliver karne ka signal deta hai.

**6. URG (Urgent)**

Urgent data ko indicate karta hai.

## 9. TCP Four-Way Handshake

TCP connection close karne ke liye normally Four-Way Termination process use hota hai.

### Step 1 — FIN

Client server ko FIN packet send karta hai.

Iska matlab hai ke client data sending complete kar chuka hai.

### Step 2 — ACK

Server client ki FIN request acknowledge karta hai.

### Step 3 — FIN

Server apni taraf se FIN packet send karta hai.

Iska matlab hai ke server bhi connection close karna chahta hai.

### Step 4 — ACK

Client final ACK send karta hai.

Ab TCP connection close ho jata hai.

### Four-Way Termination Diagram

Client                         Server

   |                              |
   | -------- FIN -------------> |
   |                              |
   | <-------- ACK ------------- |
   |                              |
   | <-------- FIN ------------- |
   |                              |
   | -------- ACK -------------> |
   |                              |
   |       Connection Closed     |

## 10. TCP and UDP Port Numbers

Port numbers applications aur services ko identify karne ke liye use hote hain.

TCP aur UDP dono port numbers use karte hain.

| Protocol | Port Number |
|---|---|
| HTTP | TCP 80 |
| HTTPS | TCP 443 |
| FTP | TCP 20, 21 |
| SSH | TCP 22 |
| DNS | UDP 53 (usually) |
| DNS Zone Transfer | TCP 53 |
| DHCP Server | UDP 67 |
| DHCP Client | UDP 68 |
| SMTP | TCP 25 |
| POP3 | TCP 110 |
| IMAP | TCP 143 |

## 11. TCP Flow Control

Flow Control aik mechanism hai jo sender ki data transmission speed ko receiver ki capacity ke mutabiq manage karta hai.

Iska purpose receiver ko overload hone se bachana hai.

TCP flow control ke liye Sliding Window mechanism use karta hai.

### Example

Agar receiver aik waqt mein limited data receive kar sakta hai to sender apni transmission us capacity ke mutabiq manage karta hai.

## 12. TCP Congestion Control

Congestion Control network traffic ko manage karta hai.

Jab network mein bohat zyada traffic hota hai to packets delay ya loss ho sakte hain.

TCP congestion control ki madad se transmission rate adjust karta hai.

### Main Concepts

- Slow Start
- Congestion Avoidance
- Fast Retransmit
- Fast Recovery

## 13. TCP Error Control

TCP data transmission mein errors aur missing segments ko detect karne mein help karta hai.

### Main Functions

- Checksum
- Acknowledgment
- Retransmission
- Sequence Numbers

Agar sender ko required acknowledgment receive nahi hota to TCP missing data retransmit kar sakta hai.

## 14. Real-Life Examples of TCP and UDP

### TCP Real-Life Example

Jab hum internet se PDF ya software download karte hain to data correctly receive hona important hota hai.

TCP reliable transmission provide karta hai.

### UDP Real-Life Example

Jab hum live video call karte hain to speed important hoti hai.

UDP low overhead communication provide karta hai.

Agar aik chhota packet miss ho jaye to video call usually continue karti rehti hai.

## 15. Advantages of TCP

- Reliable communication.
- Data correct order mein receive hota hai.
- Missing data retransmit hota hai.
- Error recovery support karta hai.
- Flow control provide karta hai.
- Congestion control support karta hai.

## 16. Advantages of UDP

- Fast communication.
- Low overhead.
- No connection establishment delay.
- Real-time applications ke liye useful.
- Simple communication mechanism.

## 17. TCP and UDP in Cybersecurity

TCP aur UDP ko cybersecurity mein understand karna bohat important hai.

Network security professionals in protocols ko traffic analysis aur troubleshooting ke liye use karte hain.

### TCP Security

- TCP connections ko monitor kiya ja sakta hai.
- Firewall TCP ports ko control kar sakta hai.
- SYN Flood aik TCP-based attack hai.
- Unauthorized connections ko detect kiya ja sakta hai.

### UDP Security

- UDP traffic ko firewall rules se control kiya ja sakta hai.
- UDP Flood aik denial-of-service attack hai.
- Open UDP ports security risk create kar sakte hain.
- DNS traffic ko monitor karna important hai.

## 18. Important Interview Questions

**Q1: What is the full form of TCP?**

Answer: Transmission Control Protocol.

**Q2: What is the full form of UDP?**

Answer: User Datagram Protocol.

**Q3: Which layer uses TCP and UDP?**

Answer: Transport Layer.

**Q4: Is TCP reliable?**

Answer: Yes, TCP provides reliable data delivery.

**Q5: Is UDP connection-oriented?**

Answer: No, UDP is connectionless.

**Q6: How many steps are in TCP Three-Way Handshake?**

Answer: Three Steps.

**Q7: What is the first step of Three-Way Handshake?**

Answer: SYN.

**Q8: What is the second step?**

Answer: SYN-ACK.

**Q9: What is the third step?**

Answer: ACK.

**Q10: Which protocol is used for online gaming?**

Answer: UDP is commonly used.

**Q11: Which protocol is used for reliable file transfer?**

Answer: TCP.

**Q12: What is TCP Four-Way Termination?**

Answer: It is the normal process of closing a TCP connection using FIN and ACK packets.

**Q13: What is a SYN Flood Attack?**

Answer: A denial-of-service attack that sends many SYN requests to exhaust server resources.

**Q14: What is Flow Control?**

Answer: It manages the sender's transmission rate according to the receiver's capacity.

## 19. Conclusion

TCP aur UDP networking ke important Transport Layer protocols hain.

TCP reliable communication provide karta hai jabke UDP fast communication provide karta hai.

TCP Three-Way Handshake connection establish karta hai aur Four-Way Termination connection close karne mein help karta hai.

In concepts ko understand karna networking, system administration aur cybersecurity ke liye bohat important hai.

**End of Networking Class 08**
