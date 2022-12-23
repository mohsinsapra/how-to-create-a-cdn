# How to Create A CDN(Cotent Delivery Network)


To create a CDN you need only three things.

    • A subdomain or a domain
    • Multiple regional servers. Virtual or dedicated.
    • A geoDNS. The tool routes domain requests to nearby servers.

First of all configure a sub main or a domain for your CDN. For the servers, You must rent servers in your audience's regions and countries. If your project is global, choose any global hosting provider. Now, You need a geoDNS DNS server to direct clients to the right server when they request the domain or subdomain. GeoDNS uses the client's IP or the recursive DNS server IP to process DNS requests. The geoDNS uses the IP to determine the user's country. GeoIP is needed.
Based on the client's location, geoDNS returns the nearest CDN server's IP address. We can build our own GeoDNS but we can use cloudfare’s geoDNS or any other ready made. Lastly, you can use ngix for your static content delivery. 

