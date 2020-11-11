# Computer Networking

## Internet Protocol Stack: 5 layers

![](.gitbook/assets/image%20%286%29.png)

Example:

![](.gitbook/assets/image%20%2814%29.png)

## What happen when we type a URL?



1. Browser checks cache for DNS \(Domain Name System\) entry to find the corresponding [IP address](https://www.geeksforgeeks.org/introduction-of-classful-ip-addressing/) of website. \(In short, use DNS to translate URL to IP address to make sure it reaches the right destination\) It looks for following cache. If not found in one, then continues checking to the next until found.
   * Browser Cache
   * Operating Systems Cache
   * Router Cache
   * ISP Cache
2. If not found in cache, ISP’s \(Internet Service Provider\) DNS server **initiates a DNS query to find IP address of server that hosts the domain name.** The requests are sent using small data packets that contain information content of request and IP address it is destined for.
3. Browser initiates a [TCP \(Transfer Control Protocol\)](https://www.geeksforgeeks.org/tcp-and-udp-in-transport-layer/) connection with the server using synchronize\(SYN\) and acknowledge\(ACK\) messages. Three-ways handshake.  ![](.gitbook/assets/image%20%2813%29.png) 
4. Browser sends an [HTTP](https://www.geeksforgeeks.org/http-non-persistent-persistent-connection/) request to the web server. **GET** or POST request.
5. Server on the host computer handles that request and **sends back a response**. It assembles a response in some format like JSON, [XML](https://www.geeksforgeeks.org/xml-basics/) and HTML.
6. Server sends out an HTTP response along with the status of response.
7. Browser displays [HTML](https://www.geeksforgeeks.org/html-tutorials/) content
8. Finally, Done.



