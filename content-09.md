# Networking Class 09 — Data, Frontend/Backend, aur Firewall

## 1. Introduction

Is class mein hum samjhein ge ke data kya hota hai, frontend aur backend kaise kaam karte hain, aur firewall network ko kis tarah secure karta hai.

Ye concepts websites, applications aur network security mein bohat important hain.

## 2. What is Data?

**Definition:** Data is a collection of raw facts and information that can be stored, processed, and transferred.

Data ka matlab information hota hai jo computer mein store, process aur transfer ki jati hai.

### Examples of Data

- User name
- Password
- Images
- Videos
- Documents
- Emails
- Messages
- Bank details

### Types of Data

1. Text Data — Names, messages aur documents.
2. Numeric Data — Numbers, prices aur account balances.
3. Image Data — Photos aur pictures.
4. Audio Data — Voice recordings aur music.
5. Video Data — Videos aur movies.

## 3. How Data Travels on a Network

Jab hum internet par kisi ko message ya file send karte hain to data network ke through travel karta hai.

### Data Transfer Process

1. Sender data send karta hai.
2. Data network ke through travel karta hai.
3. Data packets mein divide ho sakta hai.
4. Network devices data ko destination tak forward karte hain.
5. Receiver data receive karta hai.

### Real-Life Example

Jab hum WhatsApp par kisi friend ko picture send karte hain:

- Hum picture select karte hain.
- Application picture ko send karti hai.
- Data internet ke through travel karta hai.
- Receiver ke mobile par picture receive hoti hai.

## 4. What is Frontend?

**Definition:** Frontend is the part of a website or application that users can see and interact with.

Frontend website ka wo part hota hai jo user ko screen par nazar aata hai.

### Frontend Examples

- Website design
- Buttons
- Images
- Login forms
- Navigation menus
- Text and colors

### Frontend Technologies

**1. HTML**

HTML ka full form HyperText Markup Language hai.

HTML website ka structure banane ke liye use hoti hai.

**2. CSS**

CSS ka full form Cascading Style Sheets hai.

CSS website ko design aur beautiful banane ke liye use hoti hai.

**3. JavaScript**

JavaScript website ko interactive banati hai.

Example: Button click karne par koi action perform hona.

## 5. What is Backend?

**Definition:** Backend is the server-side part of an application that handles data, business logic, and database operations.

Backend website ka wo part hota hai jo background mein kaam karta hai.

User normally backend ko directly nahi dekh sakta.

### Backend Responsibilities

- User login verification
- Password checking
- Data processing
- Database management
- Server communication
- User authentication
- Data security

### Backend Technologies

- Python
- PHP
- Java
- Node.js
- Ruby

### Real-Life Example

Jab user kisi website par login karta hai:

1. User username aur password enter karta hai.
2. Frontend login information backend ko send karta hai.
3. Backend database se information check karta hai.
4. Agar information correct ho to login successful hota hai.
5. Agar information wrong ho to error show hota hai.

## 6. Difference Between Frontend and Backend

| Frontend | Backend |
|---|---|
| User ko nazar aata hai | Background mein kaam karta hai |
| Website ka design hota hai | Website ka logic handle karta hai |
| HTML, CSS, JavaScript | Python, PHP, Java, Node.js |
| User interaction handle karta hai | Data processing handle karta hai |
| Browser mein display hota hai | Server par execute hota hai |

## 7. What is a Database?

**Definition:** A database is an organized collection of data that can be stored, managed, and accessed easily.

Database data ko organized form mein store karta hai.

### Examples

- MySQL
- PostgreSQL
- MongoDB
- Microsoft SQL Server
- Amazon DynamoDB

### Database Functions

- Data store karna
- Data update karna
- Data delete karna
- Data search karna
- Data manage karna

## 8. What is a Server?

**Definition:** A server is a computer or software that provides services or resources to other computers called clients.

Server client ki requests receive karta hai aur unko response provide karta hai.

### Example

Jab hum Google open karte hain:

1. Browser Google server ko request send karta hai.
2. Server request process karta hai.
3. Server response send karta hai.
4. Google website hamari screen par display ho jati hai.

## 9. What is a Firewall?

**Definition:** A firewall is a network security system that monitors and controls incoming and outgoing network traffic based on security rules.

Firewall ek security system hai jo network traffic ko monitor aur control karta hai.

Ye decide karta hai ke kaunsa traffic allow karna hai aur kaunsa block karna hai.

### Functions of Firewall

1. Unauthorized access ko block karta hai.
2. Incoming traffic ko monitor karta hai.
3. Outgoing traffic ko control karta hai.
4. Network ko suspicious connections se protect karta hai.
5. Security rules apply karta hai.
6. Network attacks ka risk kam karne mein help karta hai.

## 10. Types of Firewall

### 1. Packet Filtering Firewall

Ye firewall network packets ko rules ke according check karta hai.

Example:
IP address aur port number check karke traffic allow ya block karna.

### 2. Stateful Inspection Firewall

Ye active network connections ki information track karta hai.

Is se firewall samajh sakta hai ke traffic kisi valid connection ka part hai ya nahi.

### 3. Proxy Firewall

Proxy firewall client aur internet ke darmiyan intermediary ka kaam karta hai.

Ye requests ko inspect karke security provide karta hai.

### 4. Next-Generation Firewall (NGFW)

NGFW advanced security features provide karta hai.

Is mein application control, intrusion prevention aur deep packet inspection jaisi capabilities ho sakti hain.

## 11. Types of Firewall Based on Deployment

### 1. Hardware Firewall

Hardware firewall ek physical device hota hai jo network ko protect karta hai.

Example: Office ya company ke network ke gateway par firewall device.

### 2. Software Firewall

Software firewall computer ya server par install hota hai.

Example: Windows Defender Firewall.

### 3. Cloud Firewall

Cloud firewall cloud infrastructure aur applications ke network traffic ko protect karta hai.

Example: AWS Network Firewall.

## 12. What is Incoming and Outgoing Traffic?

### Incoming Traffic

Incoming traffic wo data hota hai jo bahar ke network se hamare computer ya server ki taraf aata hai.

Example:
Kisi user ka website server ko request send karna.

### Outgoing Traffic

Outgoing traffic wo data hota hai jo hamare computer ya server se bahar ke network ki taraf jata hai.

Example:
Website server ka user ko webpage send karna.

## 13. What is a Firewall Rule?

Firewall rule ek security instruction hoti hai jo decide karti hai ke network traffic allow hoga ya block.

### Example

- Allow HTTP traffic on port 80.
- Allow HTTPS traffic on port 443.
- Block unauthorized connections.
- Allow SSH access only from trusted IP addresses.

## 14. Common Network Ports

| Port | Protocol | Purpose |
|---|---|---|
| 20/21 | FTP | File Transfer |
| 22 | SSH | Secure Remote Login |
| 25 | SMTP | Email Sending |
| 53 | DNS | Domain Name Resolution |
| 80 | HTTP | Website Communication |
| 443 | HTTPS | Secure Website Communication |
| 3306 | MySQL | Database Communication |

## 15. Frontend, Backend, Database and Firewall Working Together

Jab user kisi website ko open karta hai to different components mil kar kaam karte hain.

### Working Process

1. User browser mein website open karta hai.
2. Frontend user ko website ka interface show karta hai.
3. User koi request perform karta hai.
4. Backend request receive aur process karta hai.
5. Backend database se required information access karta hai.
6. Firewall network traffic ko security rules ke according control karta hai.
7. Server response frontend ko send karta hai.
8. Frontend result user ko show karta hai.

## 16. Real-Life Example — Online Shopping Website

Socho hum kisi online shopping website par mobile phone buy karte hain.

- Frontend: Products aur shopping buttons show karta hai.
- Backend: Order process karta hai.
- Database: Products aur customer information store karta hai.
- Server: Website ki requests handle karta hai.
- Firewall: Unauthorized network traffic ko control karta hai.

Is tarah ye tamam components mil kar website ko properly work karwate hain.

## 17. Why is Firewall Important in Cybersecurity?

Firewall cybersecurity ka important part hai.

Is ke benefits:

1. Unauthorized access se protection.
2. Network traffic monitoring.
3. Suspicious connections ko block karna.
4. Internal network ki security.
5. Security policies implement karna.

**Important:** Firewall akela complete security provide nahi karta. Antivirus, strong passwords, MFA, software updates aur other security controls bhi zaroori hain.

## 18. Interview Questions

**Q1: What is Data?**

Data is a collection of raw facts and information.

**Q2: What is Frontend?**

Frontend is the visible part of a website or application.

**Q3: What is Backend?**

Backend is the server-side part that handles application logic and data.

**Q4: What is a Database?**

A database is an organized collection of data.

**Q5: What is a Server?**

A server provides services or resources to clients.

**Q6: What is a Firewall?**

A firewall monitors and controls network traffic based on security rules.

**Q7: What is the difference between Frontend and Backend?**

Frontend handles the user interface, while backend handles server-side processing.

**Q8: What is Incoming Traffic?**

Incoming traffic is data coming into a computer or network.

**Q9: What is Outgoing Traffic?**

Outgoing traffic is data going out from a computer or network.

**Q10: Name some types of Firewalls.**

Packet Filtering, Stateful Inspection, Proxy Firewall and Next-Generation Firewall.

## 19. Conclusion

Is class mein hum ne Data, Frontend, Backend, Database, Server aur Firewall ke concepts samjhe.

Frontend user ko website show karta hai, backend background mein processing karta hai, database information store karta hai aur server requests handle karta hai.

Firewall network traffic ko monitor aur control karke unauthorized access se protection provide karta hai.

Ye tamam concepts networking aur cybersecurity seekhne ke liye bohat important hain.
