
# Networking Class 02 - Client-Server Model and Request Process

## 1. Introduction to Client-Server Model

### Definition

The Client-Server Model is a network architecture in which a client requests a service or resource, and a server processes the request and provides a response.

### Explanation

Client-Server Model mein client woh device ya application hoti hai jo kisi service ya information ki request karti hai. Server woh computer ya system hota hai jo request ko receive karta hai, process karta hai aur response send karta hai.

### Real-Life Example

Jab hum Google par koi cheez search karte hain:

- Humara computer ya mobile client hota hai.
- Google ke servers request receive karte hain.
- Server search results process karke response send karta hai.
- Results humari screen par show ho jate hain.

Is process mein client request karta hai aur server response deta hai.

## 2. What Is a Client?

### Definition

A client is a computer, device, or application that requests services or resources from a server.

### Explanation

Client woh device ya application hoti hai jo server se data, files ya kisi service ki request karti hai.

### Examples of Client

- Laptop par web browser.
- Mobile phone par application.
- Email application.
- Online banking application.
- Computer par FTP client.

### Functions of a Client

- Server ko request send karna.
- Server se response receive karna.
- User ko information display karna.
- User ke input ko request mein convert karna.

### Real-Life Example

Jab aap mobile par YouTube open karte hain aur koi video play karte hain, to YouTube application client ka role perform karti hai.

## 3. What Is a Server?

### Definition

A server is a computer or software system that receives requests from clients and provides services or resources.

### Explanation

Server aik computer ya software system hota hai jo clients ki requests receive karta hai aur unhein required information ya service provide karta hai.

Server files, websites, databases, emails aur doosri services provide kar sakta hai.

### Types of Servers

#### 1. Web Server

Web server websites aur web pages ko clients tak pohanchata hai.

Example: Apache HTTP Server aur Nginx.

#### 2. File Server

File server network par files store aur share karta hai.

Example: Office ka shared file server.

#### 3. Database Server

Database server data ko store, manage aur retrieve karta hai.

Example: MySQL database server.

#### 4. Mail Server

Mail server emails send, receive aur store karne mein madad karta hai.

Example: Organization ka email server.

#### 5. Application Server

Application server applications ki processing aur services provide karta hai.

### Functions of a Server

- Client ki request receive karna.
- Request ko process karna.
- Database ya files se required data lena.
- Client ko response send karna.
- Access permissions aur security rules apply karna.

## 4. Difference Between Client and Server

| Client | Server |
|---|---|
| Service ya data ki request karta hai. | Request receive karke service ya data provide karta hai. |
| User ke device par ho sakta hai. | Dedicated computer ya cloud system par ho sakta hai. |
| Response receive karta hai. | Response send karta hai. |
| Example: Web browser. | Example: Web server. |

## 5. What Is a Request?

### Definition

A request is a message sent by a client to a server asking for a resource or service.

### Explanation

Request woh message hota hai jo client server ko send karta hai. Is message mein client batata hai ke usay kya chahiye.

### Examples

- Website open karne ki request.
- Login karne ki request.
- Video play karne ki request.
- Database se data hasil karne ki request.
- File download karne ki request.

### Real-Life Example

Jab aap browser mein `www.example.com` enter karte hain, to browser website ka content hasil karne ke liye server ko request bhejta hai.

## 6. What Is a Response?

### Definition

A response is a message sent by a server back to a client after processing a request.

### Explanation

Response woh jawab hota hai jo server client ki request process karne ke baad send karta hai.

Response mein requested data, error message ya request ka status ho sakta hai.

### Examples

- Website ka page display hona.
- Login successful ka message.
- File download hona.
- Access denied ka message.
- Page not found ka error.

## 7. Client-Server Request Process

Client-server communication mein aam tor par yeh steps follow hote hain.

### Step 1: Client Sends a Request

Client kisi service ya information ki request karta hai.

Example: User browser mein website ka address enter karta hai.

### Step 2: Request Travels Through the Network

Request network ke zariye server tak pohanchti hai. Is process mein router aur doosre networking devices madad kar sakte hain.

### Step 3: Server Receives the Request

Server request receive karta hai aur check karta hai ke client ko kya chahiye.

### Step 4: Server Processes the Request

Server request ko process karta hai. Zaroorat parne par database se data hasil karta hai ya application run karta hai.

### Step 5: Server Sends a Response

Server requested information ya suitable status ke saath response client ko send karta hai.

### Step 6: Client Displays the Result

Client response receive karta hai aur user ko result show karta hai.

## 8. Request Process Example: Opening a Website

Maan lein aap browser mein `https://example.com` open karte hain.

1. Aap website ka address browser mein enter karte hain.
2. Browser DNS ke zariye domain name ka IP address maloom kar sakta hai.
3. Browser server ke saath network connection establish karta hai.
4. HTTPS connection mein secure communication ke liye TLS use hota hai.
5. Browser HTTP request server ko send karta hai.
6. Server request process karta hai.
7. Server HTTP response send karta hai.
8. Browser response mein mojood website content ko display karta hai.

### Important Point

DNS ka kaam domain name ko IP address ke saath resolve karna hai. HTTP request website ka content mangne ke liye use hoti hai. HTTPS, HTTP communication ko TLS ke zariye secure karta hai.

## 9. What Is HTTP?

### Definition

HTTP stands for Hypertext Transfer Protocol. It is an application-layer protocol used for communication between web clients and web servers.

### Explanation

HTTP aik protocol hai jo browser aur web server ke darmiyan requests aur responses ke rules define karta hai.

Jab aap website open karte hain, browser HTTP request send kar sakta hai aur server HTTP response return karta hai.

### Common HTTP Methods

#### GET

GET method server se data hasil karne ke liye use hota hai.

Example: Website ka page open karna.

#### POST

POST method server ko data send karne ke liye use hota hai.

Example: Login form submit karna.

#### PUT

PUT method kisi resource ko create ya replace karne ke liye use ho sakta hai.

#### DELETE

DELETE method kisi resource ko delete karne ki request karta hai.

## 10. What Is HTTPS?

### Definition

HTTPS stands for Hypertext Transfer Protocol Secure. It uses TLS to help protect communication between a client and a server.

### Explanation

HTTPS website aur user ke browser ke darmiyan data ko transit mein encrypt karne mein madad karta hai.

Is se network par data ko unauthorized logon ke liye read ya modify karna mushkil hota hai.

### Example

Jab aap online banking website par login karte hain, to HTTPS connection aapke browser aur website ke darmiyan communication ko protect karne mein madad karta hai.

### HTTP vs HTTPS

| HTTP | HTTPS |
|---|---|
| Communication mein TLS protection built-in nahi hoti. | TLS ke zariye communication protect hoti hai. |
| Data transit mein encrypted hona zaroori nahi. | Data transit mein encrypt hota hai. |
| Sensitive information ke liye akela munasib nahi. | Secure websites aur sensitive communication ke liye use hota hai. |

## 11. What Is a Port Number?

### Definition

A port number is a number used to identify a network service or application endpoint on a device.

### Explanation

IP address network par device tak pohanchne mein madad karta hai, jabke port number device par specific service ya application tak communication pohanchane mein madad karta hai.

### Common Port Numbers

| Port | Service |
|---|---|
| 80 | HTTP |
| 443 | HTTPS |
| 22 | SSH |
| 53 | DNS |
| 25 | SMTP |

### Example

Agar browser HTTPS website se connect karta hai, to aam tor par server ka destination port 443 hota hai.

## 12. What Is a Web Browser?

### Definition

A web browser is a client application used to access and display websites.

### Explanation

Web browser aik application hai jo websites open karne aur web content display karne ke liye use hoti hai.

### Examples

- Google Chrome
- Mozilla Firefox
- Microsoft Edge
- Safari

Browser server ko request send karta hai aur response mein milne wale web content ko display karta hai.

## 13. Advantages of Client-Server Model

- Centralized data management mumkin hoti hai.
- Data aur resources multiple clients ke saath share kiye ja sakte hain.
- Security policies central server par manage ki ja sakti hain.
- Data ka backup central system par manage karna asaan ho sakta hai.
- Server resources ko zaroorat ke mutabiq scale kiya ja sakta hai.

## 14. Disadvantages of Client-Server Model

- Server fail hone se us par depend karne wali services unavailable ho sakti hain.
- Server ki maintenance aur management ki zaroorat hoti hai.
- Zyada clients ki wajah se server par load barh sakta hai.
- Infrastructure aur security par cost aa sakti hai.
- Network problem ki wajah se client server tak nahi pohanch sakta.

## 15. Client-Server Model in AWS

AWS mein bhi client-server model use hota hai.

### Example

Maan lein aik company AWS par website host karti hai.

- **Client:** User ka browser.
- **Amazon Route 53:** Domain name ko DNS ke zariye resolve kar sakta hai.
- **Amazon EC2:** Virtual server jahan website application run ho sakti hai.
- **Application:** Client ki request process karti hai.
- **Database:** Zaroorat ke mutabiq application data hasil ya save karti hai.
- **Response:** Website ka result browser ko send hota hai.

Is tarah AWS cloud services ki madad se client-server applications host aur manage ki ja sakti hain.

## 16. Important Terms

- **Client:** Request karne wala device ya application.
- **Server:** Request process karke service provide karne wala system.
- **Request:** Client ka bheja hua message.
- **Response:** Server ka jawab.
- **HTTP:** Web communication protocol.
- **HTTPS:** TLS-protected HTTP communication.
- **DNS:** Domain name ko IP address ke saath resolve karne wala system.
- **IP Address:** Network par device ya interface ko identify karne wala address.
- **Port Number:** Network service ya application endpoint ko identify karne wala number.
- **Web Browser:** Website access karne wali client application.

## 17. Short Questions and Answers

### Q1: What is the Client-Server Model?

Yeh aik network architecture hai jahan client request karta hai aur server service ya data provide karta hai.

### Q2: What is a client?

Client woh device ya application hai jo server se service ya data ki request karti hai.

### Q3: What is a server?

Server woh system hai jo client ki request receive aur process karke response deta hai.

### Q4: What is a request?

Request client ka bheja hua message hota hai jo kisi resource ya service ko mangta hai.

### Q5: What is a response?

Response server ka jawab hota hai jo client ko send kiya jata hai.

### Q6: What is HTTP?

HTTP aik application-layer protocol hai jo web clients aur servers ke darmiyan communication ke rules define karta hai.

### Q7: What is HTTPS?

HTTPS, HTTP communication ko TLS ke zariye secure karta hai.

### Q8: What is DNS?

DNS domain names ko IP addresses ke saath resolve karne mein madad karta hai.

### Q9: What is a port number?

Port number device par network service ya application endpoint ko identify karne mein madad karta hai.

### Q10: Give an example of the Client-Server Model.

Browser se website open karna aik example hai, jahan browser request karta hai aur web server response deta hai.

## 18. Conclusion

Client-Server Model networking ka aik important concept hai. Is model mein client request send karta hai aur server us request ko process karke response deta hai.

Web browsing, online banking, email, cloud computing aur bohat si applications isi tarah client-server communication use karti hain. Request process ko samajhna networking, cybersecurity aur AWS cloud computing seekhne ke liye zaroori hai.
