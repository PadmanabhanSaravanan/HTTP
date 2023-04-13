# HTTP

![image logo](images/logo.png)

## TABLE OF CONTENT 

1. [**Introduction to HTTP**](#introduction-to-http)<!-- style="font-size:20px" -->
2. **HTTP Parameters**<!-- style="font-size:20px" -->
3. **HTTP Messages**<!-- style="font-size:20px" -->
4. **HTTP Requests**<!-- style="font-size:20px" -->
5. **HTTP Responses**<!-- style="font-size:20px" -->
6. **HTTP Methods**<!-- style="font-size:20px" -->
7. **HTTP Status Codes**<!-- style="font-size:20px" -->
8. **HTTP Header Fields**<!-- style="font-size:20px" -->
9. **HTTP Cookies**<!-- style="font-size:20px" -->
10. **HTTP Chaching**<!-- style="font-size:20px" -->
11. **HTTP URL Encoding**<!-- style="font-size:20px" -->
12. **HTTP Security**<!-- style="font-size:20px" -->


## Introduction to HTTP

* [**What is HTTP**](#what-is-http)<!-- style="font-size:20px" -->
* [**Features of HTTP**](#features-of-http)<!-- style="font-size:20px" -->
* [**HTTP Architecture**](#http-architecture)<!-- style="font-size:20px" -->
* [**Advantages of HTTP**](#advantages-of-http)<!-- style="font-size:20px" -->
* [**Disadvantages of HTTP**](#disadvantages-of-http)<!-- style="font-size:20px" -->

### **What is HTTP**

* HTTP stands for Hyper Text Transfer Protocol
* The primary function of HTTP is to establish a connection with the server and send HTML pages back to the user's browser.
* HTTP is an application protocol that runs on top of the TCP/IP suite of protocols, which forms the foundation of the internet.

![image http](images/http.png)

### **Features of HTTP**

There are three basic features of HTTP 

* **HTTP is connectionless** : The HTTP client, i.e., a browser initiates an HTTP request and after a request is made, the client waits for the response. The server processes the request and sends a response back after which client disconnect the connection. So client and server knows about each other during current request and response only. Further requests are made on new connection like client and server are new to each other.
* **HTTP is media independent**: It means, any type of data can be sent by HTTP as long as both the client and the server know how to handle the data content. It is required for the client as well as the server to specify the content type using appropriate MIME-type.
* **HTTP is stateless:** As mentioned above, HTTP is connectionless and it is a direct result of HTTP being a stateless protocol. The server and client are aware of each other only during a current request. Afterwards, both of them forget about each other. Due to this nature of the protocol, neither the client nor the browser can retain information between different requests across the web pages.

### **HTTP Architecture**

The following diagram shows a very basic architecture of a web application and depicts where HTTP sits:

![image architecture](images/Architecture.png)<!-- width="250px" height="300px" -->

The HTTP protocol is a request/response protocol based on the client/server based architecture where web browsers, robots and search engines, etc. act like HTTP clients, and the Web server acts as a server.

Client
The HTTP client sends a request to the server in the form of a request method, URI, and protocol version, followed by a MIME-like message containing request modifiers, client information, and possible body content over a TCP/IP connection.

Server
The HTTP server responds with a status line, including the message's protocol version and a success or error code, followed by a MIME-like message containing server information, entity meta information, and possible entity-body content.

### **Advantages of HTTP**

1. **Addressing**: HTTP uses advanced scheme of addressing. It assigns IP address with recognizable names so that it can be identified easily in the World Wide Web. Compared to the standard procedure of IP address with a series of numbers, using this the public can easily engage with the internet.

2. **Flexibility** : Whenever there are additional capabilities needed by an application, HTTP has the capability to download extensions or plugins and display the relevant data. These can include Flash players and Acrobat reader.

3. **Security** : In HTTP each files is downloaded from an independent connection and then gets closed. Due to this no more than one single element of a webpage gets transferred. Therefore, the chance of interception during transmission is minimized here. 
 

4. **Latency** : Only when the connection is established, the handshaking process will take place in HTTP. Hence, there will be no handshaking procedure following a request. This significantly reduces latency in the connection. 

5. **Accessibility** : When the page is loaded for the first time, all of the HTTP pages gets stored inside the internet caches known as the page cache. Therefore, once the page is visited again, the content is loaded quickly.

### **Disadvantages of HTTP**

1. **Data Integrity** : Since there are no any encryption methods used in HTTP, there are chances of someone altering the content. That is the reason why HTTP is considered to be an insecure method prone to data integrity.
2. **Data Privacy** : Privacy is another problem faced in a HTTP connection. If any hacker manages to intercept the request they can view all the content present in the web page. Besides that they can also gather confidential informations such as the username and the password.

3. **Server Availability** : Even if HTTP receives all the data that it needs, clients does not take measures to close the connection. Therefore, during this time period, server will not be present. 

4. **Administrative Overhead** : For transmitting a web page, a HTTP needs to create multiple connections. This causes administrative overhead in the connection. 
 
5. **IoT Device Support** : HTTP uses more number of system resources which leads to more power consumption. Since IoT device today contain wireless sensor networks, it is not suitable to use HTTP. 