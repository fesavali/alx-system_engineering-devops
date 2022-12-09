0x08. Networking basics #1

In the Internet Protocol Version 4, the address 0.0.0.0 is a non-routable meta-address used to designate an invalid, unknown or non-applicable target. It may also be used for when the client is offline. This address is assigned specific meanings in a number of contexts, such as on clients or on servers.
A way to specify "any IPv4 address at all". It is used in this way when configuring servers (i.e. when binding listening sockets). This is known to TCP programmers as INADDR_ANY. (bind(2) binds to addresses, not interfaces.)
The address a host claims as its own when it has not yet been assigned an address. Such as when sending the initial DHCPDISCOVER packet when using DHCP.
The address a host assigns to itself when address request via DHCP has failed, provided the host's IP stack supports this. This usage has been replaced with the APIPA mechanism in modern operating systems.
A way to explicitly specify that the target is unavailable.
A way to route a request to a nonexistent target instead of the original target. Often used for adblocking purposes.
In the context of servers, 0.0.0.0 can mean "all IPv4 addresses on the local machine". If a host has two IP addresses, 192.168.1.1 and 10.1.2.1, and a server running on the host is configured to listen on 0.0.0.0, it will be reachable at both of those IP addresses.
