Traceroute:

Developed an ICMP traceroute and a multithreaded version of an ICMP and UDP traceroute using python to show the routers used in the path to reach the destination IP + showing network metrics such as the round time trip (RTT).

- used socket programming to send ICMP packets with increasing TTL
- used multithreading to increase the performance of the traceroute by sending and receiving request in separate threads to avoid waiting for the response received from the network
- applied synchronization technique to avoid concurrency issues using a mutex

Web Proxy:

Developed a simple HTTP web proxy server for caching the HTML files.

- opened a TCP socket listening to the HTTP port (80)
- listening for HTTP requests from client, parsing the requested file from the http header and forwarding a new HTTP request with the same requested file to the origin server
- caching the file data in memory upon receiving the response from the server
- when the same request is received again using the file data from the in-memory cache if found
