# Network Traffic Analysis Report

This report summarizes the protocols identified during a live packet capture on September 29, 2025.

### Protocols Identified:

1.  **DNS (Domain Name System):**
    * **Observation:** The capture showed a standard DNS query from my PC to a DNS server. The query requested the IP address associated with the domain name `google.com`. A response packet was observed containing the correct IP address.
    * **Purpose:** This protocol acts as the "phonebook of the internet," translating human-readable domain names into machine-readable IP addresses.

2.  **ICMP (Internet Control Message Protocol):**
    * **Observation:** After the DNS lookup, several ICMP "Echo (ping) request" packets were sent from my PC to Google's server. For each request, a corresponding "Echo (ping) reply" was received.
    * **Purpose:** ICMP is used for network diagnostics to check if a host is reachable.

3.  **HTTP (Hypertext Transfer Protocol):**
    * **Observation:** The capture showed an HTTP `GET / HTTP/1.1` request from my PC's web browser to the server at `example.com`. This was followed by a response packet from the server with a status code of `200 OK`, which contained the webpage's HTML content.
    * **Purpose:** HTTP is the foundation of data communication for the World Wide Web, used to request and transmit web pages.
