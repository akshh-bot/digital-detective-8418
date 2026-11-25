# Mission 7 — How Computers Communicate

## 1. Task / objective

To understand basic computer networking concepts, observe network information using Terminal commands, learn how DNS works, and understand what happens when a user opens a website.

## 2. Work completed

- Studied different types of computer networks: LAN, MAN and WAN.
- Learned about DNS, routers, protocols and packet switching.
- Understood the client-server model.
- Practised checking network connectivity using Terminal.
- Used DNS lookup commands to find the IP address associated with a domain.
- Studied the steps involved in opening a website.
- Learned how browsers, DNS, servers and network protocols communicate.

### Task 7.1 — Network concepts

| Concept | Explain in your own words | Example |
|---|---|---|
| LAN | A network covering a small area, such as a home, lab or office. | Home Wi-Fi network |
| MAN | A network covering a city or a large campus area. | City-wide network |
| WAN | A network covering large geographical areas. | The Internet |
| DNS | Translates a domain name into an IP address. | example.com |
| Router | Connects different networks and forwards data between them. | Home Wi-Fi router |
| Protocol | A set of rules devices follow to communicate. | HTTP, HTTPS, TCP |
| Packet switching | Data is divided into packets that travel across a network. | Sending a message over the Internet |
| Client-server | A client requests a service and a server provides it. | A browser requesting a webpage |

### Task 7.2 — Observe network information

**1. Connectivity test**

Command:
`ping -c 4 example.com`

Observations:
- 4 packets transmitted.
- 4 packets received.
- 0% packet loss.
- Average response time: 6.381 ms.

A connectivity test helps check whether my computer
can communicate with another device or website
through the network.

**2. DNS lookup**

Command:
`nslookup example.com`

Observations:
- DNS server used: 8.8.8.8
- Domain: example.com
- Returned IP addresses:
  - 104.20.23.154
  - 172.66.147.243

DNS translates a human-readable domain name into
an IP address so that the browser can locate
the correct server.

**3. Role of DNS**

When I enter a website name in a browser, DNS
helps find the IP address associated with that
domain. The browser can then communicate with
the destination server.

### Task 7.3 — What happens when you open a website?

1. The user enters a website address into the browser.
2. The browser checks whether it already has the required DNS information cached.
3. If needed, the browser requests DNS resolution to find the website's IP address.
4. The device sends a request through the network and router towards the destination server.
5. The server receives the request and processes it.
6. The server sends the requested webpage data back using network protocols such as HTTPS over TCP.
7. The browser receives the response, processes the HTML, CSS and JavaScript, and displays the webpage.

## 3. Commands / tools used

- `ping`
- `nslookup`
- Terminal
- DNS
- TCP/IP
- HTTPS
- Web browser

## 4. My understanding

A computer network allows different devices to communicate and share information. I learned that DNS converts website names into IP addresses, routers forward data between networks, and protocols establish rules for communication. I also understood how a browser communicates with a server to load a website.

## 5. Difficulties faced

Initially, I was unfamiliar with the output
displayed by ping and nslookup commands.
Understanding the DNS server information and
returned IP addresses was also confusing.

## 6. How I resolved them

I ran the commands in Terminal and carefully
observed their outputs. I understood the packet
statistics from ping and learned how nslookup
displays DNS server information and IP addresses.

## 7. Evidence / files

- `mission-07-networking/README.md` — Contains networking concepts, Terminal commands, observations and explanations of website communication.

## 8. Commit details

- Commit message: Explain networking concepts and website communication.
- The completed Mission 7 README was committed and pushed to GitHub.