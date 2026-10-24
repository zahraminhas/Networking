
# Networking Class 05 - Hexadecimal to Binary aur IPv6

## 1. Introduction

Networking mein IP addresses ko samajhne ke liye number systems ka knowledge bohat important hai. Hexadecimal aur Binary number systems computers aur networking protocols mein use hotay hain.

IPv6 aik modern Internet Protocol hai jo IPv4 ke muqablay mein bohat bara address space provide karta hai.

### Topics Covered

- Number Systems
- Binary Number System
- Decimal Number System
- Hexadecimal Number System
- Hexadecimal to Binary Conversion
- Binary to Hexadecimal Conversion
- IPv6 Introduction
- IPv6 Address Structure
- IPv6 Address Shortening
- IPv6 Address Types
- IPv4 vs IPv6
- Practical Commands

## 2. Number System

### Definition

A number system is a method of representing numbers using a set of digits and a base.

### Roman Urdu Explanation

Number system numbers ko represent karne ka aik tareeqa hai. Computer science mein different number systems use hotay hain, jin mein Binary, Decimal aur Hexadecimal important hain.

### Types of Number Systems

1. Binary Number System
2. Decimal Number System
3. Hexadecimal Number System
4. Octal Number System

## 3. Binary Number System

### Definition

The binary number system is a base-2 number system that uses only two digits: 0 and 1.

### Roman Urdu Explanation

Binary system mein sirf do digits hotay hain: 0 aur 1. Computers digital information ko binary form mein process karte hain.

Binary digit ko bit kaha jata hai.

### Example

```text
Binary: 1010
```

Binary number `1010` ki decimal value:

```text
1 × 8 + 0 × 4 + 1 × 2 + 0 × 1 = 10
```

Is liye:

```text
1010 (Binary) = 10 (Decimal)
```

### Binary Place Values

Right se left ki taraf place values hoti hain:

```text
128  64  32  16  8  4  2  1
```

Example:

```text
00001010
```

Is mein 8 aur 2 wali positions par 1 hai.

```text
8 + 2 = 10
```

Is liye `00001010` ki decimal value 10 hai.

## 4. Decimal Number System

### Definition

The decimal number system is a base-10 number system that uses digits from 0 to 9.

### Roman Urdu Explanation

Decimal woh number system hai jo hum daily life mein use karte hain. Is mein 10 digits hotay hain: 0, 1, 2, 3, 4, 5, 6, 7, 8 aur 9.

### Example

```text
25 (Decimal)
```

Is number ko place values se samjhein:

```text
2 × 10 + 5 × 1 = 25
```

## 5. Hexadecimal Number System

### Definition

The hexadecimal number system is a base-16 number system that uses sixteen symbols: 0-9 and A-F.

### Roman Urdu Explanation

Hexadecimal system mein 16 symbols use hotay hain. Is mein 0 se 9 tak digits aur A se F tak letters hotay hain.

Hexadecimal networking mein khas taur par IPv6 addresses ko represent karne ke liye use hota hai.

### Hexadecimal Values

| Hexadecimal | Decimal |
|---|---:|
| 0 | 0 |
| 1 | 1 |
| 2 | 2 |
| 3 | 3 |
| 4 | 4 |
| 5 | 5 |
| 6 | 6 |
| 7 | 7 |
| 8 | 8 |
| 9 | 9 |
| A | 10 |
| B | 11 |
| C | 12 |
| D | 13 |
| E | 14 |
| F | 15 |

### Example

```text
A = 10
B = 11
C = 12
D = 13
E = 14
F = 15
```

Hexadecimal mein `A` decimal 10 ko aur `F` decimal 15 ko represent karta hai.

## 6. Hexadecimal to Binary Conversion

### Important Rule

Har hexadecimal digit ko exactly 4 binary bits mein convert kiya ja sakta hai.

### Hexadecimal to Binary Table

| Hex | Binary |
|---|---|
| 0 | 0000 |
| 1 | 0001 |
| 2 | 0010 |
| 3 | 0011 |
| 4 | 0100 |
| 5 | 0101 |
| 6 | 0110 |
| 7 | 0111 |
| 8 | 1000 |
| 9 | 1001 |
| A | 1010 |
| B | 1011 |
| C | 1100 |
| D | 1101 |
| E | 1110 |
| F | 1111 |

### Example 1: Hexadecimal 5 to Binary

Hexadecimal digit:

```text
5
```

Binary value:

```text
0101
```

Answer:

```text
5 (Hex) = 0101 (Binary)
```

### Example 2: Hexadecimal A to Binary

Hexadecimal digit:

```text
A
```

A ki decimal value 10 hai.

Binary value:

```text
1010
```

Answer:

```text
A (Hex) = 1010 (Binary)
```

### Example 3: Hexadecimal 2F to Binary

Hexadecimal number:

```text
2F
```

Har digit ko alag convert karein:

```text
2 = 0010
F = 1111
```

Ab dono binary groups ko combine karein:

```text
2F = 00101111
```

Answer:

```text
2F (Hex) = 00101111 (Binary)
```

### Example 4: Hexadecimal B7 to Binary

```text
B = 1011
7 = 0111
```

Combine karein:

```text
B7 = 10110111
```

Answer:

```text
B7 (Hex) = 10110111 (Binary)
```

## 7. Binary to Hexadecimal Conversion

### Important Rule

Binary number ko right se 4-4 bits ke groups mein divide karein. Har group ko hexadecimal digit mein convert karein.

Agar left side par 4 bits ka group complete na ho, to zaroorat ke mutabiq left side par zeros add karein.

### Example 1: Binary 1010 to Hexadecimal

Binary:

```text
1010
```

Table ke mutabiq:

```text
1010 = A
```

Answer:

```text
1010 (Binary) = A (Hex)
```

### Example 2: Binary 11001111 to Hexadecimal

Step 1: Four-bit groups banayein.

```text
1100 1111
```

Step 2: Har group convert karein.

```text
1100 = C
1111 = F
```

Answer:

```text
11001111 (Binary) = CF (Hex)
```

### Example 3: Binary 10110101 to Hexadecimal

Groups:

```text
1011 0101
```

Conversion:

```text
1011 = B
0101 = 5
```

Answer:

```text
10110101 (Binary) = B5 (Hex)
```

## 8. IPv6 Introduction

### Definition

IPv6 stands for Internet Protocol version 6. It uses 128-bit addresses to identify interfaces and support IP communication.

### Roman Urdu Explanation

IPv6 Internet Protocol ka aik version hai jo IPv4 ke muqablay mein bohat bara address space provide karta hai.

IPv4 sirf 32-bit addresses use karta hai, jabke IPv6 128-bit addresses use karta hai.

IPv6 ko is liye develop kiya gaya ke internet par bohat zyada devices ko address karne ke liye bara address space available ho.

### Example of IPv6 Address

```text
2001:0db8:0000:0000:0000:ff00:0042:8329
```

Ye aik example IPv6 address hai jo documentation aur learning ke liye use hota hai.

## 9. IPv6 Address Structure

### Definition

An IPv6 address consists of 128 bits, written as eight groups of four hexadecimal digits separated by colons.

### Roman Urdu Explanation

IPv6 address mein total 128 bits hotay hain. Isay aam tor par 8 groups mein likha jata hai.

Har group mein 4 hexadecimal digits hotay hain.

Har hexadecimal digit 4 bits represent karta hai.

Is liye:

```text
8 groups × 16 bits = 128 bits
```

### Example

```text
2001:0db8:0000:0000:0000:ff00:0042:8329
```

Is address ke 8 groups hain:

1. 2001
2. 0db8
3. 0000
4. 0000
5. 0000
6. ff00
7. 0042
8. 8329

Har group 16 bits ka hai.

### IPv6 Address Space

IPv6 mein 128-bit addresses hotay hain.

Total possible bit patterns:

```text
2^128
```

Ye address space IPv4 ke 32-bit address space se bohat zyada bara hai.

## 10. IPv6 Address Shortening

### Definition

IPv6 address shortening is a method of writing an IPv6 address in a shorter valid form by removing leading zeros and compressing a consecutive sequence of zero groups.

### Rule 1: Leading Zeros Remove Karna

Har group ke start mein mojood zeros remove kiye ja sakte hain.

Example:

```text
Original:
2001:0db8:0000:0000:0000:0000:0000:0001
```

Leading zeros remove karne ke baad:

```text
2001:db8:0:0:0:0:0:1
```

### Rule 2: Consecutive Zero Groups Compress Karna

Do ya zyada consecutive zero groups ko `::` se replace kiya ja sakta hai.

Example:

```text
2001:db8:0:0:0:0:0:1
```

Short form:

```text
2001:db8::1
```

### Important Rule

`::` aik IPv6 address mein sirf aik martaba use kiya ja sakta hai, warna original address ko uniquely reconstruct karna mushkil ho sakta hai.

## 11. IPv6 Address Types

### 1. Unicast

Unicast address aik specific interface ko identify karta hai. Packet aik destination interface ko deliver karne ke liye hota hai.

Example:

```text
2001:db8::10
```

Ye documentation ke liye reserved prefix ka example hai.

### 2. Multicast

Multicast address interfaces ke aik group ko identify karta hai. Packet group ke interested members tak deliver kiya ja sakta hai.

IPv6 multicast addresses ka prefix:

```text
ff00::/8
```

### 3. Anycast

Anycast address multiple interfaces ko assign kiya ja sakta hai. Packet aam tor par routing ke mutabiq us group ke kisi aik suitable, usually nearest, interface tak deliver hota hai.

### Important Point

IPv6 mein broadcast address nahi hota. Is ke bajaye multicast ka use hota hai.

## 12. Important IPv6 Address Ranges

### 1. Global Unicast

Global unicast addresses aam tor par public IPv6 communication ke liye use hotay hain.

Common range:

```text
2000::/3
```

### 2. Link-Local

Link-local addresses aik local network link par communication ke liye use hotay hain.

Range:

```text
fe80::/10
```

Ye addresses routers ke zariye aam tor par doosray links par forward nahi kiye jatay.

### 3. Unique Local Address

Unique local addresses private IPv6 networking ke liye use hotay hain.

Range:

```text
fc00::/7
```

Practically, locally assigned unique local addresses aksar `fd00::/8` range mein hotay hain.

### 4. Loopback

IPv6 loopback address:

```text
::1
```

Ye local device ko khud address karta hai.

### 5. Unspecified Address

IPv6 unspecified address:

```text
::
```

Ye unspecified address ko represent karta hai. Isay normal destination address ke tor par assign nahi kiya jata.

## 13. IPv4 vs IPv6

| Feature | IPv4 | IPv6 |
|---|---|---|
| Address Length | 32 bits | 128 bits |
| Number System | Decimal notation | Hexadecimal notation |
| Format | Four decimal octets | Eight hexadecimal groups |
| Separator | Dot (.) | Colon (:) |
| Example | 192.168.1.10 | 2001:db8::10 |
| Address Space | 2^32 | 2^128 |
| Broadcast | Supported | Broadcast nahi hota |
| Address Configuration | Manual ya DHCPv4 | Manual, SLAAC, DHCPv6 aur doosray methods |
| ARP | IPv4 mein use hota hai | ARP ki jagah Neighbor Discovery Protocol use hota hai |

## 14. IPv6 Address Configuration

### Static Configuration

IPv6 address manually configure kiya ja sakta hai.

### SLAAC

SLAAC ka full form Stateless Address Autoconfiguration hai.

Is mechanism mein IPv6 host router advertisements aur network prefix ki information use karke apna address configure kar sakta hai.

### DHCPv6

DHCPv6 aik protocol hai jo IPv6 network configuration provide kar sakta hai.

Network design ke mutabiq SLAAC, DHCPv6 ya dono ka combination use ho sakta hai.

### Important Point

IPv6 address configuration har network mein aik jaisi nahi hoti. Ye router advertisements aur network ki settings par depend karti hai.

## 15. IPv6 and Neighbor Discovery Protocol

### Definition

Neighbor Discovery Protocol (NDP) is an IPv6 protocol that helps nodes discover neighbors, routers and link-layer address information on a local link.

### Roman Urdu Explanation

IPv6 mein Neighbor Discovery Protocol local network par doosray nodes aur routers ko discover karne mein help karta hai.

Ye IPv4 ke ARP ke kuch functions ke equivalent functionality provide karta hai, lekin is ke additional functions bhi hain.

### Main Functions

1. Neighbor discovery.
2. Router discovery.
3. Prefix discovery.
4. Address resolution.
5. Neighbor reachability detection.

### Important Point

IPv4 mein ARP use hota hai, jabke IPv6 mein address resolution ke liye NDP use hota hai.

## 16. IPv6 Practical Commands

### Windows

IPv6 configuration check karne ke liye:

```cmd
ipconfig
```

Detailed configuration ke liye:

```cmd
ipconfig /all
```

IPv6 address ko ping karne ke liye:

```cmd
ping -6 ::1
```

Ye local IPv6 loopback address test karta hai.

### Linux

Network interfaces aur IPv6 addresses check karne ke liye:

```bash
ip -6 addr
```

IPv6 routes check karne ke liye:

```bash
ip -6 route
```

Local IPv6 loopback test karne ke liye:

```bash
ping -6 ::1
```

## 17. Common Mistakes

1. IPv4 ko 128-bit samajhna. IPv4 32-bit hota hai.
2. IPv6 ko 32-bit samajhna. IPv6 128-bit hota hai.
3. Hexadecimal mein A-F ko ignore karna.
4. Har IPv6 group ko 8 bits samajhna. Har hexadecimal group 16 bits ka hota hai.
5. IPv6 mein `::` ko aik se zyada martaba use karna.
6. IPv6 mein broadcast address samajhna. IPv6 broadcast use nahi karta.
7. IPv4 ke ARP ko IPv6 mein directly use karna. IPv6 mein NDP use hota hai.

## 18. Practice Questions

### Question 1

Hexadecimal A ki binary value kya hai?

Answer:

```text
1010
```

### Question 2

Hexadecimal F ki binary value kya hai?

Answer:

```text
1111
```

### Question 3

Hexadecimal 2F ko binary mein convert karein.

Answer:

```text
00101111
```

### Question 4

Binary 11001111 ko hexadecimal mein convert karein.

Answer:

```text
CF
```

### Question 5

IPv4 address kitne bits ka hota hai?

Answer:

```text
32 bits
```

### Question 6

IPv6 address kitne bits ka hota hai?

Answer:

```text
128 bits
```

### Question 7

IPv6 mein kitne hexadecimal groups hotay hain?

Answer:

```text
8 groups
```

### Question 8

IPv6 loopback address kya hai?

Answer:

```text
::1
```

### Question 9

IPv6 mein ARP ki jagah kaunsa protocol address resolution mein help karta hai?

Answer:

```text
Neighbor Discovery Protocol (NDP)
```

### Question 10

Kya IPv6 broadcast support karta hai?

Answer:

```text
Nahi. IPv6 multicast use karta hai.
```

## 19. Quick Revision

- Binary: Base-2 number system.
- Decimal: Base-10 number system.
- Hexadecimal: Base-16 number system.
- Hexadecimal digits: 0-9 aur A-F.
- 1 hexadecimal digit: 4 bits.
- IPv4: 32-bit address.
- IPv6: 128-bit address.
- IPv6 groups: 8 hexadecimal groups.
- IPv6 separator: Colon (:).
- IPv6 shortening: Leading zeros remove karna aur zero groups compress karna.
- IPv6 loopback: ::1
- IPv6 link-local range: fe80::/10
- IPv6 multicast range: ff00::/8
- IPv6 address resolution: NDP.

## 20. Conclusion

Hexadecimal aur binary number systems computer networking mein important role play karte hain. Har hexadecimal digit four binary bits represent karta hai, jis se IPv6 addresses ko samajhna aur convert karna asan hota hai.

IPv6 128-bit addressing use karta hai aur IPv4 ke muqablay mein bohat bara address space provide karta hai. IPv6 address structure, shortening, address types aur configuration methods samajhna modern networking ke liye zaroori hai.
