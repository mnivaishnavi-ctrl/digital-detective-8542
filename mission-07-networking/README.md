# Mission 7 – How Computers Communicate

## Task 7.1 – Network Concepts

1. **LAN (Local Area Network):** Connects devices in a small area.  
   Example: Home Wi-Fi.

2. **MAN (Metropolitan Area Network):** Connects networks across a city.  
   Example: City-wide university network.

3. **WAN (Wide Area Network):** Connects networks over large geographical areas.  
   Example: Internet.

4. **DNS (Domain Name System):** Converts domain names into IP addresses.  
   Example: google.com.

5. **Router:** Connects networks and forwards data.  
   Example: Home Wi-Fi router.

6. **Protocol:** Rules that allow devices to communicate.  
   Example: HTTP, HTTPS.

7. **Packet Switching:** Divides data into small packets for transmission.

8. **Client-Server:** Client requests services and server provides them.  
   Example: Browser requesting a webpage.

### What I Learned
I learned how computer networks work and how devices communicate and share information over the Internet.


### Task 7.2 — Network observations

I used ping to check whether example.com could be reached. Four packets were sent and received with no packet loss in this check. The result can change on a different network or at another time.

I used nslookup to find the network addresses for example.com. A DNS lookup shows the IP address linked to a domain name. DNS helps the browser find the website's server when I enter its name.

### Task 7.3 — What happens when I open a website?

1. I enter a website name in the browser. The browser is the client.
2. DNS finds the IP address linked to the website name.
3. The browser sends a request using HTTPS.
4. The request travels through my network and router toward the server.
5. The server receives the request and sends the website data back in packets.
6. The browser receives the response and displays the webpage.

## 4. Commands / tools used

- ping -c 4 example.com — checked whether the example website could be reached.
- nslookup example.com — looked up the website's network addresses.
- Terminal — ran both network commands.

## 5. My understanding

DNS helps a browser find a server using a website name. The client sends a request, and the server sends a response. A router helps move data between networks.

## 6. Difficulties faced

No major difficulties.

## 7. How I resolved them

Not applicable.

## 8. Evidence / files

- This README has the network concepts and observations.
- evidence/network-checks.txt has the command results. It does not include my own IP address or Wi-Fi details.

## 9. Commit details

Commit message: Explain networking concepts and website communication

The Mission 7 work was pushed to GitHub.