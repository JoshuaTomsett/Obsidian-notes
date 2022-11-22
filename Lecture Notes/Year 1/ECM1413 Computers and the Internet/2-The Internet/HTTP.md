[[ECM1413 Computers and the Internet]]

17-Nov-2022


### Application Layer

Examples:
- HTTP
- FTP
- SMTP
- SSH
- DNS


#### Client-server protocols

![[Pasted image 20221117195852.png]]

In HTTP, a client sends a request for a web page to a server and recieves the page as a response back from it.


#### HTTP Requests

- The request line
- The request heads
- The request body


![[Pasted image 20221117200145.png]]
![[Pasted image 20221117200202.png]]
![[Pasted image 20221117200211.png]]
![[Pasted image 20221117200223.png]]
![[Pasted image 20221117200231.png]]


#### HTTP Responses

- The status line
- The response headers
- The response body


![[Pasted image 20221117200346.png]]
![[Pasted image 20221117200355.png]]
![[Pasted image 20221117200405.png]]
![[Pasted image 20221117200415.png]]


### Loading a Web Page

A client examines a recieved HTML file and looks for references to other files, and then sends HTTP requests for these as well

Files that are found in the web cache do not need to be requested


### HTTPS

All requests and responses are encrypted

Authentification proves that the server is the legitimate host of the website

