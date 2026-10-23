
# Networking Class 03 - IP Address, Types, Public/Private, NAT

## 1. Introduction to IP Address

### Definition

An IP (Internet Protocol) address is a logical address used to identify a device or network interface and help deliver data across an IP network.

### Explanation

IP address aik logical address hota hai jo network par device ko identify karne aur data ko sahi destination tak pohanchane mein madad karta hai.

Jaise ghar tak letter pohanchane ke liye ghar ka address chahiye hota hai, isi tarah network par data ko destination tak pohanchane ke liye IP address use hota hai.

### Example

`192.168.1.10`

Yeh IPv4 address ki aik example hai jo home network mein kisi device ko assign ho sakti hai.

### Uses of IP Address

- Network par devices ko identify karna.
- Data ko destination tak pohanchane mein madad dena.
- Different networks ke darmiyan communication karna.
- Internet aur local network services use karna.
- Network troubleshooting mein madad dena.

## 2. Types of IP Addresses

IP addresses ko mukhtalif tareeqon se classify kiya jata hai.

### 1. IPv4 Address

IPv4 ka full form Internet Protocol Version 4 hai.

IPv4 aik 32-bit addressing system hai. Is mein 4 numbers hote hain jo dots se separate kiye jate hain.

**Example:** `192.168.1.10`

Har number ki value 0 se 255 tak hoti hai.

IPv4 mein taqreeban 4.3 billion addresses ki theoretical range hoti hai, lekin tamam addresses normal devices ko assign nahi kiye ja sakte.

### 2. IPv6 Address

IPv6 ka full form Internet Protocol Version 6 hai.

IPv6 aik 128-bit addressing system hai jo IPv4 ke muqable mein bohat zyada addresses provide karta hai.

**Example:** `2001:db8::1`

IPv6 addresses hexadecimal format mein likhe jate hain aur colons se separate hote hain.

### IPv4 and IPv6 Difference

| IPv4 | IPv6 |
|---|---|
| 32-bit address use karta hai. | 128-bit address use karta hai. |
| Example: `192.168.1.10` | Example: `2001:db8::1` |
| Dots use karta hai. | Colons use karta hai. |
| Address space comparatively chhoti hai. | Address space bohat zyada hai. |

## 3. Public IP Address

### Definition

A public IP address is an IP address that is globally routable on the public internet.

### Explanation

Public IP address internet par communication ke liye use hota hai. Internet Service Provider (ISP) aam tor par internet connection ke saath public IP address provide karta hai.

Public IP address ki madad se internet par dusre systems aapke network ya internet-facing service tak pohanch sakte hain, agar routing aur security rules ijazat dein.

### Example

Maan lein kisi company ke web server ke paas public IP address hai. Internet users us server ki website tak pohanch sakte hain, agar server aur firewall ki configuration allow kare.

### Uses of Public IP Address

- Internet-facing websites host karna.
- Public servers tak internet se pohanchna.
- Internet par devices ya network services ke saath communication karna.

### Important Point

Public IP address hone ka matlab yeh nahi ke device automatically secure ya har kisi ke liye accessible hai. Firewall, routing aur doosri security settings bhi matter karti hain.

## 4. Private IP Address

### Definition

A private IP address is an IP address reserved for use inside private networks and is not directly routable across the public internet.

### Explanation

Private IP address ghar, office, school ya organization ke local network mein devices ko assign kiya jata hai.

Misal ke taur par mobile, laptop aur printer ko router private IP addresses assign kar sakta hai.

### Example

- `192.168.1.10`
- `192.168.1.20`
- `10.0.0.5`

### IPv4 Private IP Ranges

Private IPv4 addresses ke 3 main ranges hain:

| Private Range | Address Range |
|---|---|
| Class A private range | `10.0.0.0` se `10.255.255.255` |
| Class B private range | `172.16.0.0` se `172.31.255.255` |
| Class C private range | `192.168.0.0` se `192.168.255.255` |

Yeh ranges private IPv4 networking ke liye reserved hain.

### Uses of Private IP Address

- Home network mein devices connect karna.
- Office ke computers ko network par identify karna.
- Local printers aur servers ko connect karna.
- Internal applications aur services chalana.

### Advantages of Private IP Address

- Internal network ke liye addresses provide karta hai.
- Public IPv4 addresses ki zaroorat kam karta hai.
- Internal devices ko directly public IP dene ki zaroorat nahi hoti.
- Network ko organize aur manage karne mein madad karta hai.

## 5. Difference Between Public and Private IP

| Public IP | Private IP |
|---|---|
| Public internet par globally routable hota hai. | Private network ke andar use hota hai. |
| Aam tor par ISP provide karta hai. | Router ya network administrator assign kar sakta hai. |
| Internet-facing services ke liye use ho sakta hai. | Local devices aur internal services ke liye use hota hai. |
| Internet par unique routing address hota hai. | Different private networks mein same address dobara use ho sakta hai. |
| Example: ISP ka diya hua public address. | Example: `192.168.1.10` |

## 6. What Is NAT?

### Definition

NAT stands for Network Address Translation. It is a networking technique that translates IP addresses as packets pass through a router or firewall.

### Explanation

NAT aik technique hai jis mein router ya firewall network traffic ke IP addresses ko translate karta hai.

Home networks mein NAT aksar private IP addresses ko public IP address ke zariye internet par communicate karne mein madad karta hai.

### Real-Life Example

Maan lein ghar mein 3 devices hain:

- Mobile: `192.168.1.10`
- Laptop: `192.168.1.20`
- Tablet: `192.168.1.30`

Yeh devices private IP addresses use karte hain. Jab yeh internet par communication karte hain, to home router aam tor par NAT aur connection tracking ke zariye unki traffic ko aik public IPv4 address ke through bhej sakta hai.

Router translation aur port information ki madad se incoming responses ko mutaliqa internal device tak wapas pohanchata hai.

### Why Is NAT Used?

- Multiple private IPv4 devices ko public IPv4 address ke zariye internet use karne dena.
- Public IPv4 addresses ki zaroorat kam karna.
- Internal aur external addressing ke darmiyan translation karna.

### Important Point

NAT khud complete security solution nahi hai. Network ko protect karne ke liye firewall rules, secure configuration aur doosri security practices bhi zaroori hain.

## 7. Types of NAT

### 1. Static NAT

Static NAT mein aik private IP address ko aik specific public IP address ke saath permanently map kiya jata hai.

**Example:**

Private IP: `192.168.1.10`

Public IP: `203.0.113.10`

Yeh example documentation ke liye reserved public address range use karti hai.

Static NAT mein mapping aam tor par fixed rehti hai.

**Use:** Aise internal server ko specific public address ke saath map karna jise bahar se access karna ho.

### 2. Dynamic NAT

Dynamic NAT mein private IP addresses ko available public IP addresses ke pool se temporarily map kiya jata hai.

Is mein mapping available addresses aur network configuration ke mutabiq change ho sakti hai.

**Use:** Jab organization ke paas public IP addresses ka pool ho aur woh unhein internal devices ke liye use karna chahe.

### 3. PAT (Port Address Translation)

PAT ko NAT Overload bhi kaha jata hai.

Is mein multiple private devices aik public IPv4 address share kar sakte hain. Router different connections ko identify karne ke liye port numbers use karta hai.

**Example:**

- Mobile: `192.168.1.10`
- Laptop: `192.168.1.20`
- Tablet: `192.168.1.30`

Yeh teeno devices aik hi public IPv4 address ke zariye internet use kar sakte hain, jab router PAT support aur configuration use kar raha ho.

### Types of NAT Difference

| Static NAT | Dynamic NAT | PAT |
|---|---|---|
| Fixed address mapping. | Public IP pool se mapping. | Aksar aik public IP multiple devices share karte hain. |
| Aam tor par one-to-one mapping. | Available public addresses par depend karta hai. | Port numbers connections ko distinguish karte hain. |
| Specific server mapping mein useful. | Address pool wali networks mein useful. | Home aur office internet sharing mein common. |

## 8. How NAT Works Step by Step

Maan lein aapka laptop internet par website open karna chahta hai.

### Step 1: Device Sends Data

Laptop apne private IP address se website ki request send karta hai.

Example: `192.168.1.20`

### Step 2: Traffic Reaches the Router

Data router tak pohanchta hai. Router packet ke source aur destination addresses ko check karta hai.

### Step 3: NAT Translation Happens

Router apni NAT configuration ke mutabiq source address ko translate karta hai. PAT mein port information bhi use ho sakti hai.

### Step 4: Request Travels to the Internet

Translated packet internet par destination server ki taraf forward hota hai.

### Step 5: Server Sends a Response

Website ka server response send karta hai jo router tak wapas pohanchta hai.

### Step 6: Router Forwards the Response

Router apni translation aur connection information ki madad se response ko sahi internal device tak pohanchata hai.

Is tarah laptop internet par website access kar leta hai.

## 9. NAT vs Firewall

| NAT | Firewall |
|---|---|
| IP addresses ko translate karta hai. | Security rules ke mutabiq traffic allow ya block karta hai. |
| Address translation aur traffic forwarding mein role hota hai. | Unauthorized traffic ko control karne mein role hota hai. |
| Akela complete security solution nahi hai. | Security policy enforce karne ke liye use hota hai. |

Kuch routers aur firewalls NAT aur firewall dono functions perform karte hain, lekin dono ke purposes alag hain.

## 10. Public and Private IP in AWS

AWS cloud networking mein bhi public aur private IP addresses use hote hain.

### Public IP in AWS

Public IP address internet-facing resources ko public internet se communicate karne mein madad de sakta hai, agar routing aur security configuration allow kare.

Example: Public subnet mein internet-facing web server.

### Private IP in AWS

Private IP address VPC ke andar resources ke internal communication ke liye use hota hai.

Example: Private subnet mein database server.

### Example Architecture

- Public subnet mein web server ho sakta hai.
- Private subnet mein database server ho sakta hai.
- Web server database se private network ke zariye communicate kar sakta hai.
- Security groups aur network rules access ko control karte hain.
- NAT Gateway private subnet ke resources ko supported configuration mein outbound internet access de sakta hai.

### Important AWS Point

AWS mein public subnet ka matlab sirf yeh nahi ke resource ke paas public IP hai. Subnet ki route table mein internet gateway ki route aur resource ki public addressing aur security configuration bhi matter karti hai.

Private subnet ke resources outbound internet ke liye NAT Gateway use kar sakte hain, lekin NAT Gateway apne aap inbound internet connections initiate karne ki ijazat nahi deta.

## 11. Important Terms

- **IP Address:** Network par device ya interface ko identify karne wala logical address.
- **IPv4:** 32-bit IP addressing system.
- **IPv6:** 128-bit IP addressing system.
- **Public IP:** Public internet par globally routable IP address.
- **Private IP:** Private network ke liye reserved IP address.
- **NAT:** Network Address Translation.
- **Static NAT:** Fixed address mapping.
- **Dynamic NAT:** Public IP pool se address mapping.
- **PAT:** Port numbers ke zariye multiple connections ko aik public IP share karne dena.
- **Router:** Networks ke darmiyan data packets forward karne wala device.
- **Firewall:** Network traffic ko security rules ke mutabiq control karne wala system.

## 12. Short Questions and Answers

### Q1: What is an IP address?

IP address aik logical address hai jo network par devices ki identification aur data delivery mein madad karta hai.

### Q2: What is IPv4?

IPv4 aik 32-bit addressing system hai.

### Q3: What is IPv6?

IPv6 aik 128-bit addressing system hai.

### Q4: What is a public IP address?

Public IP address internet par globally routable address hota hai.

### Q5: What is a private IP address?

Private IP address internal private networks mein use hota hai aur public internet par directly routable nahi hota.

### Q6: What is NAT?

NAT aik technique hai jo network packets mein IP addresses ko translate karti hai.

### Q7: What is Static NAT?

Static NAT private aur public IP addresses ke darmiyan fixed mapping banata hai.

### Q8: What is Dynamic NAT?

Dynamic NAT available public IP pool se private addresses ki mapping karta hai.

### Q9: What is PAT?

PAT multiple private devices ko aik public IPv4 address share karne deta hai, port numbers ki madad se.

### Q10: Does NAT replace a firewall?

Nahi. NAT aur firewall ke functions alag hain. Network security ke liye firewall rules bhi zaroori ho sakte hain.

## 13. Conclusion

IP address networking ka important hissa hai kyun ke yeh devices aur network interfaces ki identification aur data delivery mein madad karta hai.

IPv4 aur IPv6 IP addressing ke do versions hain. Public IP internet par globally routable hota hai, jabke private IP internal networks mein use hota hai.

NAT private aur public addressing ke darmiyan translation karta hai aur IPv4 networks mein multiple devices ko internet use karne mein madad de sakta hai. In concepts ko samajhna networking, cybersecurity aur AWS cloud networking seekhne ke liye zaroori hai.
