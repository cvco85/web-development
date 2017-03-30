# Introduction to web development

A gentle introdution about the basics of the web

## How the internet works?

[![How the internet works](http://img.youtube.com/vi/7_LPdttKXPc/0.jpg)](https://www.youtube.com/watch?v=7_LPdttKXPc)

Take offs:

- The internet is a wire
- There are servers, clients, and resources
- IP addresses are identifiers
- ISPs are the "middle man"
- DNS are "translators" from IPs to urls
- Emails are an example of a resource that travels "through" the wire
- Information is sent through packets (TCP)
- Routers now how to direct packets to their route

## Web protocols

1. HTTP
2. HTTPS

### HTTP/HTTPS (HyperText Transfer Protocol)

![http][howHttpWorks]
Clients and servers communicate by exchanging individual messages (as opposed to a stream of data). The messages sent by the client, usually a Web browser, are called requests and the messages sent by the server as an answer are called responses.

[howHttpWorks]: https://mdn.mozillademos.org/files/13677/Fetching_a_page.png

![network][networkHttp]
HTTP is an extensible protocol which has evolved over time. It is an application layer 
protocol that is sent over TCP, or over a TLS-encrypted TCP connection.

[networkHttp]: https://mdn.mozillademos.org/files/13673/HTTP%20&%20layers.png

#### Difference between http and https

Encryption, vulnerability to MiM attacks. Http uses port 80, https uses 443.

___

### Components

#### Client: User-agent

Is normally the browser, the tool that acts on befalt of the user. The one that initiates the request (in the majority of the cases).

The browser nows how to get and interpret different resources (HTML, CSS, videos, scripts). Deals mainly with HTTP/HTTPS requests.

#### Server

On the other side of the communication, *serves and/or generates* the document requested by the cleint. Presents himself as a single machine virtually (in reality it could be a lot more than one, for the same purpose). 

#### Proxies

"Men in the middle". Completely transparent for the HTTP protocol, can be things that handle network protocols, caching, filtering, load balancing, authentication or logging.

- Simple
- Extensible
- Stateless but not sessionless

___

### What really happens?

```
→ curl www.flag.pt -v | /dev/null
zsh: permission denied: /dev/null
* Rebuilt URL to: www.flag.pt/
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0*   Trying 192.199.26.1...
* Connected to www.flag.pt (192.199.26.1) port 80 (#0)
> GET / HTTP/1.1
> Host: www.flag.pt
> User-Agent: curl/7.43.0
> Accept: */*
>
< HTTP/1.1 200 OK
< Content-Type: text/html; charset=UTF-8
< Vary: Cookie
< Server: Microsoft-IIS/8.5
< X-Powered-By: PHP/5.6.0
< Set-Cookie: center=lisboa; expires=Sun, 28-Mar-2027 22:38:33 GMT; Max-Age=315360000; path=/
< X-Pingback: http://www.flag.pt/activeapp/xmlrpc.php
< Date: Thu, 30 Mar 2017 22:38:33 GMT
< Content-Length: 49503
<
{ [5141 bytes data]
 10 49503   10  5141    0     0   4476      0  0:00:11  0:00:01  0:00:10  4478*
```

##### Request
![http request][httpRequest]

##### Response
![http response][httpResponse]

[More detail about requests and responses](https://developer.mozilla.org/en-US/docs/Web/HTTP/Session)

[httpRequest]: https://mdn.mozillademos.org/files/13687/HTTP_Request.png
[httpResponse]: https://mdn.mozillademos.org/files/13691/HTTP_Response.png

### DNS 

```
→ host google.com
google.com has address 195.8.12.103
google.com has address 195.8.12.118
google.com has address 195.8.12.88
google.com has address 195.8.12.99
google.com has address 195.8.12.94
google.com has address 195.8.12.84
google.com has address 195.8.12.104
google.com has address 195.8.12.113
google.com has address 195.8.12.93
google.com has address 195.8.12.98
google.com has address 195.8.12.123
google.com has address 195.8.12.108
google.com has address 195.8.12.114
google.com has address 195.8.12.89
google.com has address 195.8.12.109
google.com has address 195.8.12.119
google.com has IPv6 address 2a00:1450:4003:804::200e
google.com mail is handled by 30 alt2.aspmx.l.google.com.
google.com mail is handled by 20 alt1.aspmx.l.google.com.
google.com mail is handled by 40 alt3.aspmx.l.google.com.
google.com mail is handled by 50 alt4.aspmx.l.google.com.
google.com mail is handled by 10 aspmx.l.google.com.

```


#### References
___

##### TCP (Transmission Control Protocol)

Provides reliable, ordered and error checked delivery of the message. Works on the transport layer of the [IP protocol](https://en.wikipedia.org/wiki/Internet_protocol_suite).

##### TLS

Cryptographic protocols used to provide security to communications over a computer network. Used by websites to secure the communication between the client and the server.
